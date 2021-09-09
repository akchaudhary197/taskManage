# taskManage
All the api are available in server.js file with description.
req.body contain the required data from user or from frontend.
For testing purpose you can pass data from postman, but you need to create data base.

I also added data base details, I'm using mongo as a database for this tasks.
You Just need to create only one table

// Task
const mongoose = require('mongoose');

const tasks = mongoose.Schema({
    _id : mongoose.Schema.Types.ObjectId,
    name : {type : String , required : true} , 
    completed:{type : Boolean, default: false }
})

module.exports = mongoose.model('Task',tasks)

if you have any further query then reply me on same repository or mail me at akchaudhary197@gmail.com.
