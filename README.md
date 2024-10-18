Setup Instructions
Step 1: Start the Server
Open your terminal and navigate to the directory containing the server.py file. Then run the following command:

python3 server.py
Step 2: Start the Panel Server
In another terminal window, navigate to the same directory and start the panel server using the following command:

./panel-server
You can access the dashboard at http://localhost/panel.html.

Step 3: Set Up SSH Tunneling
To route traffic properly, set up SSH tunneling by running the following command in your terminal:

ssh -R 80:localhost:<PORT> (portal as server has)
Replace <PORT> with the port number used by your server. This command forwards port 80 on the remote server to your local machine.

Using the DDoS Tool
You can use a powerful Layer 7 DDoS tool for testing. The tool can be found here: ZxCDDoS. Follow the instructions in the repository to set it up and run it against a URL you want to test.
( https://github.com/hoaan1995/ZxCDDoS ) 

crash URL GET
To test the DDoS mitigation, you can use a GET request to crash a URL:
