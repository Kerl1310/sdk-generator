const sdk = require('node-appwrite');

// Init SDK
let client = new sdk.Client();

let users = new sdk.Users(client);

client
    .setProject('')
;

let promise = users.deleteUserSession('[USER_ID]', '[SESSION_ID]');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});