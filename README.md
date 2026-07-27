This file contains the content for the website parkgrovecounselling.co.uk

To run the website locally first setup the IP address using the command :
```bash
IP_ADDRESS=`hostname -I | awk '{ print $1 }'`
echo $IP_ADDRESS
```

To run the site locally use the command : 
```
hugo server --bind=0.0.0.0 --baseURL=http://$IP_ADDRESS:1313 -D
```

To build the site run the command
```bash
hugo
```
which will create the content in the directory called `public`.

To update the website copy the contents of the public directory to the repository 
[https://github.com/parkgrove-counselling/parkgrove-counselling.github.io](https://github.com/parkgrove-counselling/parkgrove-counselling.github.io)