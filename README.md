# VerifAge
VerifAge is an Age Verification Solution for Cashier-less Checkouts in Stores

What is VerifAge?
VerifAge is the solution to verify the Customer’s age, before allowing the Customer to checkout ‘age-restricted’ items in the store, through any of the cashier-less checkout options. 

What does VerifAge do?
VerifAge first asks the Customer do register a valid ID proof on the App, that could be validated and approved by an Associate/Team in the backend. 
Whenever the Customer is ready to checkout an ‘age-restricted’ item, VerifAge asks the Customer to click a photo of themselves. Then, VerifAge – 
  1. Tries to determine the age of the Customer based on the photo taken. 
  2. Compares the photo with the photo in the ID on record. 
If both of these conditions pass, then the Customer is cleared to checkout the ‘age-restricted’ item.

VerifAge - Tech Stack:
Azure Face Service:
The face detection, age detection, and face match and verification features, are leveraged from Azure Face Service.
The Azure Face service provides AI algorithms that detect, recognize, and analyse human faces in images.
The Azure Face Service allows REST API calls, that can take image payloads, and get response with the attributes of the face in the image. 
After registering a base image from a valid photo ID, the Face API can compare images clicked on the phone camera with the baselined image, and can suggest if both the faces match, and the degree of confidence. 

Shortcuts on iOS:
The Shortcuts app on iOS is an automation tool that lets you create your own shortcuts with multiple steps or actions, leveraging various features of the iPhone.
We are using the Shortcuts App as a ‘Zero Code’ platform to mount our solution on. 
The Shortcuts app allows for sending REST API calls and also allows unpacking of JSON data sent as response.
Capture/Selection of photos, and sending it as payload in the REST API calls was done through Shortcuts.

What does this Repo contain?
This Repo contains the various REST API calls that were used during the various stages of VerifAge
