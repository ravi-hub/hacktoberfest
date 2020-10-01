// GITHUB: https://github.com/ravi-hub

var Person = function(name,location){
  this.name = (name) ? name : "ravi";
  this.place = (location) ? location : "india";
}
Person.prototype.greeting = function(name){
  name = (name) ? name : this.name;
  var str = "Hello, World! by " + name;
  console.log(str);
  return str;
}
class Person {
  constructor (name='ravi', location='india') {
    this.name = name;
    this.place = location;
  }
  greeting (name=this.name) {
    let str = "Hello, World! by " + name;
    console.log(str);
    return str;
  }
}

var myself = new Person('hub','new delhi');
