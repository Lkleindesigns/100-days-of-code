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

<h2 align=”center”>
Day 3: January 3, 2018
</h2>

<img src="https://udemy-images.udemy.com/course/750x422/1286908_1773_4.jpg" alt="ReactJs">
<img src ="https://media.giphy.com/media/3ohc0TbEIU708sJhVm/giphy.gif">

**Today's Progress**: Today I created a random box app with react, which creates an array of boxes, randomly selects a box 
and randomly changes it to a different color every second. This app really helped my understanding of pure functions,
stateless functional objects, react component architecture and the intricacies of state and setState.

```
const NUM_RECT = 300;

const Rect = ({color}) => {
  const style = {
    width: '100px',
    height: '180px',
    display: 'inline-block',
    backgroundColor: color
  }
  return <div style={style} />
}

class App extends Component {
  constructor(props) {
    super(props);
    const rects = Array(NUM_RECT).fill().map(this.getRandomColor, this)
    this.state = {rects}
    
    setInterval(() => {
      const rects = this.state.rects.slice()
      const randIndex = Math.floor(Math.random() * rects.length)
      rects[randIndex] = this.getRandomColor()
      this.setState({rects})
    },300)
  }
```

**Thoughts:**: I started this exercise feeling unsure, but with research and time I overcame it. I had a lot of life distractions 
and obstacles, still I made coding my priority regardless and feel really accomplished today.

**Link to work:**: [random-boxes](https://github.com/Lkleindesigns/random-boxes/blob/master/src/App.js)

<h2 align=”center”>
Day 4: January 5, 2018
</h2>

<img src="https://scontent-dft4-2.xx.fbcdn.net/v/t31.0-8/25488302_373727013076731_1843187123777200206_o.jpg?oh=8b54791f18bb7d30291be7eb5f332147&oe=5AFAEEE2" alt="ReactJs">


**Today's Progress**: I learned a lot about the virtual DOM, synthetic events, error boundaries, and Fiber. Today didn't consist of a lot of actual code it was more research and learning.
I also committed to the Code Newbies Get a Job Challenge and completed my first assignment analyzing my own skills and researching potential future job.

**Thoughts:**: I missed a day yesterday but made up for it today!

<h2 align=”center”>
Day 5: January 6, 2018
</h2>

<img src="https://tech.io/blog/wp-content/uploads/2017/08/todolist2-1.jpg" alt="ReactJs">


**Today's Progress**: I created a very simple todo app with react, learned a lot about how to work with
click events, forms, and inputs within react. Read some of the React documentation and also refreshed my memory
on some ES6 subjects.

**Thoughts:**: I'm beginning to feel more confident with react and seeing design patterns.

**Link to work:**: [react-simple-todolist](https://github.com/Lkleindesigns/react-simple-todolist/blob/master/src/App.js)

<h2 align=”center”>
Day 6: January 7, 2018
</h2>

<img src="https://udemy-images.udemy.com/course/750x422/1049092_8c52_2.jpg">


**Today's Progress**: I updated my previous book app into a recipe app, added a form, click events, and some css, I also watched some videos and cloned a project
I have been working on with a friend using Node, Mongo and Express with jQuery. 

**Thoughts:**: Need to make the form save the data thats saved and update the virtual DOM and work more on other projects

**Link to work:**: [recipe-react-app](https://github.com/Lkleindesigns/recipe-react-app)

<h2 align=”center”>
Day 7: January 8, 2018
</h2>

<img src="https://reactjs.org/logo-og.png">


**Today's Progress**: Continued to work on the recipe react app added functionality to the form. Saving
showing and hiding, and begun working on delete functionality.

**Thoughts:**: Forms within react are complex and will take some more time to feel comfortable working with them.

**Link to work:**: [recipe-react-app](https://github.com/Lkleindesigns/recipe-react-app)
