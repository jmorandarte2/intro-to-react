 <!DOCTYPE html>
 <html>
    <head>
      <title>My React Assignment</title>
    </head>
  
    <body>
      <h1><strong>Hi! Please see my goals below!</strong></h1>
      <div id="myReactCode"></div>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/react/16.1.0/umd/react.development.js"></script>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/16.1.0/umd/react-dom.development.js"></script>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.34/browser.min.js"></script>
      <script type="text/babel">
                   class MyGoal extends React.Component {
          render() {
            return (
              <div>
                  <h2> My Goals : </h2>
                  <ul>
                  <li>Be very knowledgeable with react</li>
                  <li>Complete the bootcamp as soon as possible</li>
                  <li>Find job as a web developer</li>
                  </ul>
              </div>
            );
          }
        }
  
        ReactDOM.render(
          <MyGoal />, document.getElementById('myReactCode')
        );
      </script>
   </body>
 
 </html>