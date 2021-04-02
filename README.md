# WebRTCPeerMesh
Just a little experiment to create a Full Mesh WebRTC call. Each browser peer will have to connect to every other peer by:
1. Pressing the button "Click To Add peerConnection" (Which just runs the function "newPeer()" to create a new RTCPeerConnection object and the functions for handling teack events and connecting.
2. Then having one peer click "Connect to Peer" with the input field blank to generate an offer Session Description
3. Send that to one other peer and have them paste the offer into the input field and click connect
4. Copy and paste the answer back to the offering peer and click connect
5. Next repeat these steps for each additional peer you want to connect to
 
 If you want, you can store a pointer to each RTCPeerConnection object in an array and create dataChannel connections to enable stuff like private messaging, 
 or looping through the peerConnection objects to send a message to each dataChannel.
