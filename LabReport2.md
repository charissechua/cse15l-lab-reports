# **Lab Report 2**
**Charisse Chua**

## Part 1
Code written for `StringServer`: 
```
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
   ```
   
   Using add-message I created the following: 
   ![Image](<a href="https://www.linkpicture.com/view.php?img=LPic63d5ef43787062071634698"><img src="https://www.linkpicture.com/q/Screenshot_20230128_075735.png" type="image"></a>)
