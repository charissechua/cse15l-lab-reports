# **Lab Report 2**
**Charisse Chua**

## Part 1
Code that I wrote for `StringServer`: 
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
