class Person {
  constructor(name, job) {
    this.name = name
    this.job = job
    this.greet = () => {
      console.log(`My name ${this.name}. I am ${this.job}.`)
    }
  }
}

const person = new Person(`Julio`, `Developer`)

person.greet()

class User {
  constructor(name, job, company) {
    Person.call(this, name, job)
    this.company = company
    this.greet = () => {
      console.log(`Hi ${this.name}. Nice to know that you are a ${this.job} at ${this.company}.`)
    }
  }
}

User.prototype = Object.create(Person.prototype)

const user = new User(`Julio`, `Developer`, `Glints`)
console.log(user)

user.greet()
