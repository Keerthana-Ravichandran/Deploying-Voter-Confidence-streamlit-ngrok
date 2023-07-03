

https://nbviewer.org/github/Keerthana-Ravichandran/Python-Simulation-on-Policy-Watch-No.7-/blob/main/Python_Simulation_on_Policy_Watch_No_7.ipynb

#Click this link to view the colab notebook.

# Deploying-Winning-Voter-Confidence-paper-as-Streamlit-app-in-colab-using-ngrok

POLICY WATCH NO 7 :Winning Voter Confidence :

In Policy Watch No.7, the author argues that the current Voter Verifiable Paper Audit Trail (VVPAT)-based audit of Electronic Voting Machines (EVMs) in India is faulty.
It undermines voter confidence in the electoral process.
The author suggests that the current system of conducting VVPAT audits of EVMs is inadequate and lacks transparency,
which makes it difficult for voters to trust the election results.

WHAT IS NGROK?

It is a tool that provides secure tunnels to localhost/web servers, allowing developers to expose local development servers, APIs or webhooks to the internet securely. 
It creates a public URL (HTTP or HTTPS) for a local web server running on your machine and provides you with a way to access that web server from the internet. 
Ngrok can be useful for testing and sharing web projects, APIs, and other applications that require remote access.


HOW TO DEPLOY STREAMLIT APP IN COLAB USING NGROK?

Install Streamlit and ngrok using pip:
      !pip install streamlit pyngrok
      
Write the Streamlit app code and save it to a file (let's say app.py).Start an ngrok tunnel on the port your app is running on:
      from pyngrok import ngrok
      public_url = ngrok.connect(port='8501')
      print(public_url)
      
Open the URL displayed in the ngrok output in a new browser tab to see your deployed Streamlit app.

Note: 
The ngrok tunnel has a limited lifespan, so you will need to restart it and update the URL in your browser if you need to continue using the app after the tunnel has expired.


