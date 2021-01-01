# WebClient 
POST
```c#
        using (var wb = new WebClient())
            {
                var data = new NameValueCollection();
                data["message"] = "message";
                data["access_token"] = "access_token";

                var response = wb.UploadValues(url, "POST", data);
                string responseInString = Encoding.UTF8.GetString(response);
                Console.WriteLine("Post : Successfuly");
                Console.ReadLine();
            }
```
GET
```c#
        using (var wb = new WebClient())
            {
                var response = wb.DownloadString(url);
            }
```
Save to .txt
```c#
                using (System.IO.StreamWriter file = new System.IO.StreamWriter(@"C:\Users\66971\Desktop\Menu FacebookAuto\FacebookAuto\FacebookAuto\bin\Debug\group.txt"))
                        {
                            file.WriteLine("fds");
                        }
```
Get ReadText .txt
```c#
                string pathComment = @"C:\Users\66971\Desktop\Menu FacebookAuto\FacebookAuto\FacebookAuto\bin\Debug\FBComment.txt";
                    string[] readText = File.ReadAllLines(pathComment);
                    foreach (string CommentFB in readText)
                    {
                        Console.WriteLine(CommentFB);
                    }
                    
                    ```
