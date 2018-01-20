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

<h2 align=”center”>
Day 8: January 9, 2018
</h2>

<img src="http://bleedingcode.com/wp-content/uploads/2016/07/reactjs-javascript-banner-e1469539084683.jpg">


**Today's Progress**: Finished delete functionality for the recipe app. Began working on a memory game react app. Got basic functionality working, need to add a reset button.

**Thoughts:**: Finally feel like I have a solid understanding of writing complex ternary operators. Getting more comfortable with React little by little each day.

**Link to work:**: [recipe-react-app](https://github.com/Lkleindesigns/recipe-react-app)
**Link to work:**: [react-memory-game](https://github.com/Lkleindesigns/react-memory-game/blob/master/src/MemoryGame.js)

<h2 align=”center”>
Day 9: January 10, 2018
</h2>

**Today's Progress**: Set up a local dev environment on my PC due to having issues with Webpack on c9. Spent a few hours reading the React docs and following some examples

**Thoughts:**: Took a step backwards today to really reinforce everything that i've been learning the past week.

<h2 align=”center”>
Day 10: January 11, 2018
</h2>

**Today's Progress**: Setup environment to run and transpile JSX using babel, more time spent with the React docs. Wrote some basic JSX to make sure babel is working locally.
```
const app = {
    title: 'Indecision App',
    subtitle: 'Put your life in the hands of a computer'
}

var template = (
    <div>
        <h1>{app.title}</h1>
        <p>{app.subtitle}</p>
    </div>
)

var appRoot = document.getElementById('app')

ReactDOM.render(template, appRoot)
```

**Thoughts:**: Trusting in the process. 10 days in I can't wait to see where i'm at 100 days. Taking a few steps back to take larger strides forward!

<h2 align=”center”>
Day 11: January 12, 2018
</h2>

```
const app = {
    title: 'Indecision App',
    subtitle: 'Put your life in the hands of a computer',
    options: ['One', 'Two']
}

const template = (
    <div>
        <h1>{app.title}</h1>
        {app.subtitle && <p>{app.subtitle}</p>}
        <p>{app.options.length > 0 ? "Here are your options" : "No Options"}</p>
    </div>
)

const appRoot = document.getElementById('app')

ReactDOM.render(template, appRoot)
```

**Today's Progress**:  Practice with JSX conditional rendering, const and let, and arrow functions

**Thoughts:**: Worked an 11 hour shift today so my coding time was limited to only an hour.

<h2 align=”center”>
Day 12: January 13, 2018
</h2>

**Today's Progress**: ES6 Arrow functions, events and attributes in React, and manual data binding. Wrote a simple counter app

**Thoughts:**: I've had limited time to code the past couple days. Nothing will stop me from getting at least an hour every day, no excuses.
```
let count = 0

const addOne = () => {
    count++
    renderCounterApp()
}
const minusOne = () => {
    count--
    renderCounterApp()
}
const reset = () => {
    count = 0
    renderCounterApp()
}

const appRoot = document.getElementById('app')

const renderCounterApp = () => {
    const templateTwo = (
        <div>
            <h1>Count: {count}</h1>
            <button onClick={addOne}>+1</button>
            <button onClick={minusOne}>-1</button>
            <button onClick={reset}>reset</button>
        </div>
    )

    ReactDOM.render(templateTwo, appRoot)
}

renderCounterApp()
```

<h2 align=”center”>
Day 13: January 14, 2018
</h2>

**Today's Progress**: More practice with React basics, forms and inputs, and rendering in react.

**Thoughts:**: Feeling a lot more confident with forms and events and referencing the React docs if I get stuck.

```
const handleSubmit = (e) => {
    e.preventDefault()

    const option = e.target.elements.option.value

    if(option) {
        app.options.push(option)
        e.target.elements.option.value = ''
        renderTemplate()
    }
}

const handleRemoveAll = () => {
        app.options = []
        renderTemplate()
}

const renderTemplate = () => {
    const template = (
        <div>
            <h1>{app.title}</h1>
            {app.subtitle && <p>{app.subtitle}</p>}
            <p>{app.options.length > 0 ? "Here are your options" : "No Options"}</p>
            <p>{app.options.length}</p>
            <button onClick={handleRemoveAll}>Remove All</button>
            <ol>
                <li>Option one</li>
                <li>Option two</li>
            </ol>
            <form onSubmit={handleSubmit}>
                <input type="text" name="option" />
                <button>Add Option</button>
            </form>
        </div>
    )
    ReactDOM.render(template, appRoot)
}

const appRoot = document.getElementById('app')
renderTemplate()
```

<h2 align=”center”>
Day 14: January 15, 2018
</h2>

**Today's Progress**: Even more practice with JSX, Basic functionality for simple app working.

**Thoughts:**: Two weeks in and im proud of myself, worked another 12 hour shift today and still stayed consistent with an hour of code! No excuses.
```
const onMakeDecision = () => {
    const randomNum = Math.floor(Math.random() * app.options.length)
    const option = app.options[randomNum]
    alert(option)
}

const renderTemplate = () => {
    const template = (
        <div>
            <h1>{app.title}</h1>
            {app.subtitle && <p>{app.subtitle}</p>}
            <p>{app.options.length > 0 ? "Here are your options" : "No Options"}</p>
            <button disabled={app.options.length === 0} onClick={onMakeDecision}>What should I do?</button>
            <button onClick={handleRemoveAll}>Remove All</button>
            <ol>
                {    
                    app.options.map((option, i) => <li key={i}>{option}</li>)
                }
            </ol>
            <form onSubmit={handleSubmit}>
                <input type="text" name="option" />
                <button>Add Option</button>
            </form>
        </div>
    )
    ReactDOM.render(template, appRoot)
}

const appRoot = document.getElementById('app')
renderTemplate()
```

<h2 align=”center”>
Day 15 & 16: January 16-17, 2018
</h2>

**Today's Progress**: Built a simple visibility toggler using JSX and babel, review of ES6 classes, constructors, and the super and extends keywords.

**Thoughts:**: Feeling more confident with React fundamentals. Didn't update the log yesterday but I did code, so including yesterdays work in with today.
```
let visibility = false

const handleClick = () => {
    visibility = !visibility
    renderTemplate()
}

const renderTemplate = () => {
    const template = (
        <div>
            <h1>Visibility Toggler</h1>
            <button onClick={handleClick}>
                {visibility ? 'Hide Details' : 'Show Details'}
            </button>
            {visibility && (
                <div>
                <p>Something</p>
                </div>
            )}
        </div>
    )
    ReactDOM.render(template, document.getElementById('app'))
}

renderTemplate()
```
```
class Person {
    constructor(name='anonymous', age=0) {
        this.name = name || 'test'
        this.age = age
    }
    sayHello(){
        return `Hi! ${this.name} nice to meet you!`
    }
    getDescription(){
        return `${this.name} is ${this.age} years old`
    }
}

class Student extends Person {
    constructor(name, age, major){
        super(name, age)
        this.major = major
    }
    hasMajor() {
       return !!this.major
    }
    getDescription() {
        let description = super.getDescription()

        if(this.hasMajor()) {
            description += ` their major is ${this.major}`
        }

        return description
    }
}
```

<h2 align=”center”>
Day 17 & 18: January 18-19, 2018
</h2>

**Today's Progress**: Jam 18- Review of React components, props, events and methods. 
Jan 19 - Review of method binding within react. Lots of review and practice with the basics of state.
Started jsx counter app rework using react.

**Thoughts:**:  18th was my birthday, I still coded but did not get to update my log including it for today.
Making sure to update my log every day going forward and also writing a brief about something difficult to review if applicable.

**Brief**: 1. Providing e.preventDefault() if I am submitting any type of form. 
2. If this is used in a class method, a constructor and super need to be included to bind the this within the class.
3. Need to get more comfortable with using e.target in various events within React.
4. Clarifying where the name attribute is necessary and used within inputs and forms.
```
class Counter extends React.Component {
    constructor(props){
        super(props)
        this.handleAddOne = this.handleAddOne.bind(this)
        this.handleMinusOne = this.handleMinusOne.bind(this)
        this.handleReset = this.handleReset.bind(this)
    }
    handleAddOne(){
        console.log('Add One')
    }
    handleMinusOne(){
        console.log('Minus one')
    }
    handleReset(){
        console.log('Reset')
    }


    render(){
        return (
            <div>
                <h1>Count: </h1>
                <button onClick={this.handleAddOne}>+1</button>
                <button onClick={this.handleMinusOne}>-1</button>
                <button onClick={this.handleReset}>reset</button>
            </div>
        )
    }
}

ReactDOM.render(<Counter />, document.getElementById('app'))

```
```
class AddOption extends React.Component {
    handleAddOption(e){
        e.preventDefault()
        const option = e.target.elements.option.value.trim()

        if(option) {
            alert(option)
        }
    }
    render() {
        return(
            <div>
                <form onSubmit={this.handleAddOption}>
                    <input type='text' name='option' />
                    <button>Submit</button>
                </form>
            </div>
        )
    }
}

class Options extends React.Component {
    constructor(props){
        super(props)
        this.handleRemoveAll = this.handleRemoveAll.bind(this)
    }
    
    handleRemoveAll() {
        alert('handleRemoveAll')
    }
    
    render () {
        return (
            <div>
                <button onClick={this.handleRemoveAll}>Remove all</button>
                {
                    this.props.options.map((option, i) => <Option key={i} option={option} />)
                }
            </div>
        )
    }
}
```