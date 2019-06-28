# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs)
- React is a modern, efficient answer to complex UI applications
- React is a flexible library that plays the role of V in an MVC framework

 
 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.
 
 
 //Your Answer
 Smart components have their own state whereas dumb components do not. Limiting the amount of smart components helps clean up the program and makes it easier to edit it. 
 
 //Googled Answer
 Smart components are any components that manage their own state. Dumb components are stateless components that just draws info from the smart components.
 
#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?
 
 
 //Your Answer
 I have no idea
 
 //Googled Answer
 yarn add ... adds a package to the computer that lets it use the file.
 package.json and yarn.lock will automatically update.
 
#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:
1) extends Component
2) this.state.recipes must be an array
3) recipes declaration has to be under render. can only return 1 item

    import React, { Component } from 'react';

    class Recipes extends Component{
      constructor(props){
        super(props)
        this.state = {
          recipes:
            [{name: 'Meatballs'},
            {name: 'Mac & Cheese'}]

        }
      }

      render() {

          let recipes = this.state.recipes.map(function(recipe){
              return(
                  <li key={recipe.name}>{recipe.name}</li>
              )
          })
        return (


          <ul>
            {recipes}
          </ul>
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)
 
 //Your Answer
 input ='submit'
 
 //Googled Answer
 input ='radio'
 input ='button'
 input ='checkbox'
 
 #### 7. How would you explain state to a friend who doesn't know code?
 
 //Your Answer
 State is the memory of the program. Putting things in the state of a component allows it to remember it and any changes to it we want to make.
 
 
 //Googled Answer
 A computer program stores data in variables, which represent storage locations in the computer's memory. 
 The contents of these memory locations, at any given point in the program's execution, is called the program's state.
 
 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.
 
 
 //Your Answer
 Component state is saved and can be sent to child components to be used as a prop. As a result, props allow child components to take in info from the parent but not allowed to edit the parents' state.
 
 
 //Googled Answer
 In a React component, props are variables passed to it by its parent component. State on the other hand is still variables, but directly initialized and managed by the component.
   
#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
Didn't do the tic-tac-toe project. We did treasure hunt and battleship. We were unable to do battleship at first so we switched to treasure hunt and finished that really quickly. After that we were
able to do the battlship program relatively quickly. I learned that I should work from small steps first before I tackle something big. 