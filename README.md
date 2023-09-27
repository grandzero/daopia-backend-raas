# **Daopia Backend**

**[Daopia Backend](https://api.daopia.com)**

## **Overview**

Daopia Backend is a Node.js-based project, providing a REST API through Express.js. It serves as the backbone for the **[Daopia platform](https://github.com/grandzero/daopia)**, handling file uploads, encryption, and interacting with the blockchain. The project is developed using the **[RAAS Starter Kit](https://github.com/filecoin-project/raas-starter-kit)**.

## **Key Features**

### **Upload File Endpoint**

The most crucial endpoint in this project is **`/uploadFile`**. After a user has made a contribution request through the frontend and the contract, they upload the file by calling this endpoint. During the file upload, the endpoint sets the access condition to the Daopia contract and encrypts the file accordingly. It also selects the on-chain standards set by the DAO as the deal details.

### **Event Listening and Job Registration**

The API also listens to the events of the Deal Status contract deployed by Daopia. If a submit event occurs, or a DAO approves a proposal, it registers a job for it and performs the replication/renewal processes.

## **Setup and Deployment**

Before deploying the project, ensure that all dependencies are installed, and the environment is correctly configured.

```jsx
npm i
npm start
```

## **Contributing**

Contributions are welcome! Feel free to submit issues, create pull requests, or propose new features to enhance the functionality of the Daopia Backend.
