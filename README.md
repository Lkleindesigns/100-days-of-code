<h1 align="center">100 Days Of Code with Logan Klein</h1>

<img src="https://images.unsplash.com/photo-1454165205744-3b78555e5572?dpr=1&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=&bg=" alt="Image of laptop with code">

Hello! I am beginning a 100-day coding journey to step outside of my element and focus on my own projects.
For the past year, I have been learning Javascript and Node as well as other popular frameworks and libraries like React, Express, and Mongo.

Every day I will focus as much time as possible to improving my development skills!

<img src="#" alt="">

<p align="center"><b>Follow me on Twitter </b><a href="https://twitter.com/Klein_LoganA">here</a>.</p>

<p align="center"><b>Check out my repos </b><a href="https://github.com/Lkleindesigns">here</a>.</p>
<hr>

<h2 align=”center”>
Day 1: January 1, 2018
</h2>

<img src="https://dev.codetrick.net/wp-content/uploads/2017/05/7.png" alt="ReactJs">
<img src ="https://i.imgur.com/6tdbBJj.png">

**Today's Progress**: I've been working on creating sites and learning more about react. I worked on a simple book app to reinforce
React Prop and Component basics. I also set up a virtual wokrspace, visual log for this journey and created my first commit.

**Thoughts:**: A good exercise to reinforce react basics, I would like add state, touch up the css and images used.

**Link to work:**: [book-app](https://github.com/Lkleindesigns/book-app)

<h2 align=”center”>
Day 2: January 2, 2018
</h2>

<img src="https://ihatetomatoes.net/wp-content/uploads/2017/08/03-state-vs-props.png" alt="ReactJs">

**Today's Progress**: Started my morning with more practice in react, I completed a challenge on updating state in React in Colt Steele's Advanced Web Developer course. The 
exercise was to randomly select an object in a array of objects, then to randomly select an item in an array on the object, remove it, and update the state.
```
    setTimeout(() => {
            const randInst = Math.floor(Math.random() * this.state.instructors.length)
            const hobbyIndex = Math.floor(Math.random() * this.state.instructors[randInst].length)
            
            const instructors = this.state.instructors.map((instructor, index) => {
              if(index === randInst) {
                const hobbies = [...instructor.hobbies]
                hobbies.splice(hobbyIndex, 1)
                return {...instructor, hobbies}
              }
              return instructor
            })
            this.setState({instructors})
    },5000)
  }
```
I also created a simple counter that updates state using a function parameter.

```
class Counter extends Component {
    constructor(props) {
        super(props);
        this.state = {initialAge: 28}
        
        setInterval(()=> {
            this.setState((prevState, props) => {
               return {initialAge: prevState.initialAge + 1}
           })
        }, 5000)
        console.log(this.state.initialAge)
    }
    render(){
        const age = this.state.initialAge
        return(
            <div>
                {age}
            </div>
        )
    }
}
```

**Thoughts:**: Updating state is tricky, it has a lot of very specific rules. 

**Link to work:**: [react-counter](https://github.com/Lkleindesigns/state-practice/blob/master/src/Counter.js)