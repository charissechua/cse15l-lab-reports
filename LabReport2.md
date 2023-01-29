# **Lab Report 2**
**Charisse Chua**

## Part 1
Code written for `StringServer`: 
```
class Handler implements URLHandler {
    // The one bit of state on the server: a string that will be manipulated by
    // various requests.
    String string = "";
    public String handleRequest(URI url) {
        if(url.getPath().equals("/")){
            if (string.equals(""))
                return ("Current string is empty");
            else
                return ("Current string is " + string);
        }
        else {
            System.out.println("Path: " + url.getPath());
        if (url.getPath().contains("/add-message")) {
            String[] parameters = url.getQuery().split("=");
        if (parameters[0].equals("s")) {
                string = string.concat(parameters[1] + "\n");
                return string;
                }
            }
        }
        return "404 Not Found!";
    }

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
}
   ```
   
   Using `http://localhost:3948/add-message?s=hello` I created the following: 
   <a href="https://www.linkpicture.com/view.php?img=LPic63d5ef43787062071634698"><img src="https://www.linkpicture.com/q/Screenshot_20230128_075735.png" type="image"></a> 
   
   * Only one method, `handleRequest` is called. This method is designed to handle all of the different scenarios for this specific program in one place. The only parameter that is passed in is a `URI`, which is later broken down in the program to get necessary information on how to handle it. The most important value is the path. The first step is to compare the path to just a `/`, if the path is a `/` that means that no command has been called. Thus, I have it set to just display the current value of `string`. In this case, the path was `/add-message`, so the next value it checks is the query. It splits it into 2 values, `s` and whatever value follows `=`. If the value of `parameters[0]` does not equal `s`, then it returns `404 not found`. Because this specific request was adding a message, the field `string` is concatenated with the new string, as well as `\n` for a new line. 

 * Then added another string on the next line by `http://localhost:3948/add-message?s=world`: 
   <a href="https://www.linkpicture.com/view.php?img=LPic63d5ef43787062071634698"><img src="https://www.linkpicture.com/q/Screenshot_20230128_075747.png" type="image"></a>
   
  * Again, only one method `handleRequest` is called. It again takes `url` that was passed in and isolates the path. Since the path is again `/add-message`, it goes on to isolate the query which is `?s=world`. Because of that, the string `world` is concatenated onto the current `string` along with a new line in order to produce the output `hello world` on separate lines. 

## Part 2
**For the buggy method `reverse`:** Failure inducing input
```
@Test
  public void testReversed2() {
    int [] input2 = {1, 2, 3};
    int [] input2Reverse = {3, 2, 1};


    assertArrayEquals(input2Reverse,ArrayExamples.reversed(input2));
  }
```
Input that doesn't produce a failure: 
```

@Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
  ```
Symptom of running the two tests: 
Failure inducing input: 
<a href='https://www.linkpicture.com/view.php?img=LPic63d5f5b6e8b931048684267'><img src='https://www.linkpicture.com/q/Screenshot_20230128_082717.png' type='image'></a>
Original code: 
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
Fixed code: 
```
 static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
The original problem in the code was that it was reversing the original array and using that reversed array to continue to assign the new "reversed" values into the same array. Since there was no temporary array made this method doesn't work. The reason why it passed the second test was because the input was just an empty array, so reversing it just gives the same output. The same thing would apply if the array had only one value. By creating a temporary array I was able to fix the bug. 

## Part 3
In week 2 I learned what everything in the url actually means. I had a rough guess previously as to how the computer uses the url to do certain tasks, but it was cool to be able to write a program myself that takes the url and breaks it down. Using the query to do different tasks was really helpful and now I will know exactly what everything in the long urls on my own laptop are pointing to. 
