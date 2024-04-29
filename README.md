# chats-love-here
this is secur chat app
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>
  <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <h1>Be Privacy</h1>
    </head>
    <!DOCTYPE html>
<html>
<head>
  <title>Search Bar</title>
  <style>
    #search-container {
      text-align: center;
      margin-top: 12px;
    }
    #search-input {
      padding: 10px;
      border-radius: 1rem;
      border-color: black;
      border-top: none;
      border-left: none;
      border-right: none;
      background-color: rgb(219, 245, 236);
      color: black;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    height: 0.7rem;
    width: 2cm;
      font-size: 13px;
      width: 300px;
    }
  </style>
</head>
<body>
  <div id="search-container">
    <input type="text" id="search-input" placeholder="Quick Search">
  </div>

  <script>
    const searchInput = document.getElementById('search-input');

    searchInput.addEventListener('keydown', function(event) {
      if (event.key === 'Enter') {
        const query = searchInput.value.trim();
        if (query) {
          const googleSearchURL = `https://www.google.com/search?q=${encodeURIComponent(query)}`;
          window.open(googleSearchURL, '_blank');
        }
      }
    });
  </script>
</body>
</html>
    <nav>
    <a href="https://accounts.snapchat.com/accounts/v2/login"><img src="https://cdn-icons-png.flaticon.com/128/2175/2175225.png" alt=""></a>
    <a href="https://www.instagram.com/"><img src="https://cdn-icons-png.flaticon.com/128/3670/3670274.png" alt=""></a>
    <a href="https://www.instagram.com/"><img src="https://cdn-icons-png.flaticon.com/128/906/906794.png" alt=""></a>
    </nav>
    <body>
        <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>We Love Quite </title>
      <link rel="stylesheet" href="styles.css">
    </head>
    <style>
      h1{font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 30px;
  color: lime;
  justify-content: center;
  text-align: center;
background-color: rgba(0, 0, 0, 0.952);
border-radius: 3rem;}

nav img{width: 50px;
height: 50px;
margin-left: 1cm;
padding-right: 0.7cm;
}
    </style>
    
    <body>
      <div id="chat-container">
        <div id="chat-window"></div>
    
          <input type="text" id="message-input" placeholder="Think before type...">
       
          <button id="send-button"><img src="https://cdn-icons-png.flaticon.com/128/10747/10747272.png" alt=""></button>
        </div>
      </div>
      <script type="module" src="chat.jsx"></script>
    <script type="module" src="chat.js"></script>
    </body>
    </html>
    </body>
    </html>
  
  
  
  <script>const chatWindow = document.getElementById('chat-window');
      const messageInput = document.getElementById('message-input');
      const sendButton = document.getElementById('send-button');
      
      // Load messages from local storage
      const messages = JSON.parse(localStorage.getItem('messages')) || [];
      
      // Render messages
      function renderMessages() {
        chatWindow.innerHTML = '';
        for (const message of messages) {
          const messageElement = document.createElement('div');
          messageElement.textContent = `${message.sender}: ${message.content}`;
          chatWindow.appendChild(messageElement);
        }
      }
      
      // Save messages to local storage
      function saveMessages() {
        localStorage.setItem('messages', JSON.stringify(messages));
      }
      
      // Send message
      function sendMessage() {
        const content = messageInput.value.trim();
        if (content) {
          const message = {
            sender: '',
            content
          };
          messages.push(message);
          saveMessages();
          renderMessages();
          messageInput.value = '';
        }
      }
      
      // Event listeners
      sendButton.addEventListener('click', sendMessage);
      messageInput.addEventListener('keyup', (event) => {
        if (event.key === 'Enter') {
          sendMessage();
        }
      });
      
      // Initial render
      renderMessages();</script>
  
  
  <style>html{margin-top: 2cm;
  background-image: url('https://img.freepik.com/free-vector/simple-blue-gradient-background-vector-business_53876-140900.jpg');
  }
    
    
    #chat-container {
      max-width: 620px;
      margin-top: 0.3cm;
      border: none;
      border-radius: 10px;
    }
  
    #send-button img{width: 18px;
    height: 18px;}
    
    #chat-window {
      height: 750px;
      overflow-y: scroll;
      width: 9.3cm;
      padding: 9px;
      font-family: monospace;
      color: rgb(206, 40, 73) ;
      font-size: 24px;
      border-radius: 9px;
    
      
  
      background-image: url("https://images.pexels.com/photos/4197491/pexels-photo-4197491.jpeg?auto=compress&cs=tinysrgb&w=400");
    }

   
    
    #input-container {
  
      padding: 10px;
      margin-left: 1.2cm;
      position: fixed;
      z-index: 999;
   
     
     
      
    }
    
    #message-input {
      flex-grow: 1;
      padding: 5px;
      border: none;
      font-size: 16px;
      width: 7cm;
      border-radius: 20px;
      font-family: 'Times New Roman', Times, serif;
      color:rgb(48, 47, 47);
      background-color: rgb(245, 235, 236);
    }
  
    #message-input:hover{background-color: rgb(253, 224, 228);}
    
    #send-button {
      margin-left: 10px;
      border: none;
      padding: 5px 10px;
      font-size: 10px;
      margin-top: -7px;
      height: 30px;
      border-radius: 3rem;
      width: 1.5cm;
      padding-top: 2px;
      padding-bottom: 25px;
      background-color: rgba(125, 182, 230, 0.87);}
      
      #send-button:hover{
        background-color: rgb(247, 195, 204);
     font-size: 15px; }
    </style>
  
  
  
  
    
    
  
  
  
  
  
  
    <script>const express = require('express');
      const app = express();
      const http = require('http').createServer(app);
      const io = require('socket.io')(http);
      
      app.use(express.static('public'));
      
      io.on('connection', (socket) => {
        console.log('A user connected');
      
        socket.on('message', (data) => {
          console.log(`Received message: ${data.content} from ${data.sender}`);
          io.emit('message', data);
        });
      
        socket.on('disconnect', () => {
          console.log('A user disconnected');
        });
      });
      
      const PORT = process.env.PORT || 8000;
      http.listen(PORT, () => {
        console.log(`Server listening on port ${PORT}`);
      });</script>
  
  <script>
  
  import React, { useState, useEffect } from 'react';
  import io from 'socket.io-client';
  
  const socket = io();
  
  const ChatApp = () => {
    const [messages, setMessages] = useState([]);
    const [inputValue, setInputValue] = useState('');
  
    useEffect(() => {
      socket.on('message', (data) => {
        setMessages((prevMessages) => [...prevMessages, data]);
      });
    }, []);
  
    const sendMessage = () => {
      if (inputValue.trim()) {
        const message = {
          sender: '',
          content: inputValue.trim(),
        };
        socket.emit('message', message);
        setInputValue('');
      }
    };
  
    const handleInputChange = (e) => {
      setInputValue(e.target.value);
    };
  
    const handleKeyPress = (e) => {
      if (e.key === 'Enter') {
        sendMessage();
      }
    };
  
    return (
      <div>
        <div>
          {messages.map((message, index) => (
            <div key={index}>
              <strong>{message.sender}:</strong> {message.content}
            </div>
          ))}
        </div>
        <div>
          <input
            type="text"
            value={inputValue}
            onChange={handleInputChange}
            onKeyPress={handleKeyPress}
            placeholder="Secrate..."
          />
          <button onClick={sendMessage}>Saw</button>
        </div>
      </div>
    );
  };
  
  export default ChatApp;
  </script>
  

<script>
// Function to handle device motion events
function handleMotion(event) {
  // Check if the device was shaken or flipped
  if (event.accelerationIncludingGravity.x > 10 || event.rotationRate.alpha > 10) {
    // Change the webpage URL
    window.location.href = "https://www.google.com/";
  }
}

// Add event listener for device motion
window.addEventListener("devicemotion", handleMotion);
</script>
</body>
</html>