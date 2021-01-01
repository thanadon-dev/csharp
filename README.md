# WebClient
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
