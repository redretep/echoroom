EchoRoom

EchoRoom is a minimalist, client-side, real-time chat application inspired by tlk.io and Ephemeros Chat. It leverages WebRTC and Yjs to enable peer-to-peer communication without the need for a traditional backend server to store or relay messages. A public signaling server is used to facilitate initial peer discovery, but message data flows directly between connected clients.
Features

    🔁 Real-time Messaging: Powered by WebRTC for direct peer-to-peer communication and Yjs for collaborative data synchronization.

    📎 Image Sharing: Easily share images directly within chatrooms.

    🎤 Voice Messages: Send push-to-record voice messages (requires microphone access).

    💬 Emoji Reactions: (Placeholder) Future support for emoji reactions on messages.

    ➤ Flexible Sending: Send messages by pressing Enter or using a floating send button.

    🧠 No Login, No Server (for data): No user accounts or central message storage. All chat data is synchronized peer-to-peer.

    🎨 Minimal Design: Clean layout with a dark mode option, inspired by NothingOS aesthetics.

    💨 Smooth UI Animations: Enjoy a fluid user experience with subtle animations.

How It Works

EchoRoom utilizes the following core technologies:

    WebRTC: For establishing direct peer-to-peer connections between browsers, allowing messages and media to flow without hitting a central server.

    Yjs: A CRDT (Conflict-free Replicated Data Type) framework that enables collaborative editing and real-time synchronization of shared data structures (in this case, the chat messages array) across multiple clients.

    Signaling Server: While the message data is peer-to-peer, a small signaling server (wss://signaling.yjs.dev) is used to help peers discover each other and exchange initial connection information (like IP addresses and session descriptions). This server does not store any chat messages.

How to Use

    Create a Chatroom: Enter a name in the "New chatroom name" field and click "Create Chatroom."

    Select a Chatroom: Click on an existing chatroom from the list to join it.

    Start Chatting: Type your message in the input field and press Enter or click the send button.

    Share Images: Click the paperclip icon to upload and share an image.

    Send Voice Messages: Click and hold the microphone icon to record and send a voice message. Release to stop recording.

    Dark Mode: Toggle between light and dark mode using the moon/sun icon in the header.

To chat with others: Share the URL of your deployed EchoRoom application with friends. When they open the same URL and join the same chatroom name, their browsers will connect peer-to-peer, and messages will synchronize in real-time.
Deployment on GitHub Pages

You can easily host your EchoRoom application using GitHub Pages:

    Create a GitHub Repository:

        Go to GitHub and create a new public repository (e.g., echoroom-chat).

    Save index.html:

        Save the EchoRoom HTML code (from the Canvas or your local editor) as index.html in the root of your project directory.

    Upload to Repository:

        Upload your index.html file to the main (or master) branch of your GitHub repository.

    Enable GitHub Pages:

        Go to your repository's "Settings" tab.

        Navigate to "Pages" in the left sidebar.

        Under "Build and deployment," set "Source" to "Deploy from a branch."

        Select your main (or master) branch and choose the / (root) folder.

        Click "Save."

    Access Your Site:

        After a few minutes, your EchoRoom application will be live at https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/.

Enjoy your real-time, serverless chat experience with EchoRoom!
