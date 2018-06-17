 <!DOCTYPE html>
 <html>
    <head>
      <title>My React Assignment</title>
    </head>
  
    <body>
      <div id="myReactCode"></div>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/react/16.1.0/umd/react.development.js"></script>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/16.1.0/umd/react-dom.development.js"></script>
      <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.34/browser.min.js"></script>
      <script type="text/babel">
                   class MyGoal extends React.Component {
                     constructor() {
                       super();
                       this.state = {title: "Hi! Please see my goals below!"};
                     }
          render() {
            return (
              <div>
              <h1><strong>{this.state.title}</strong></h1>
                  <h2> My Goals :</h2> 
              <ul>
            <li> {this.props.list} </li>
            <li> {this.props.list2} </li>
            <li> {this.props.list3} </li>
              </ul>
              </div>
            );
          }
        }
        
        const info = {
          list: 'Be very knowledgeable with react',
          list2: 'Complete the bootcamp as soon as possible',
          list3: 'Find job as a web developer',
        }
  
        ReactDOM.render(
          <MyGoal list = {info.list}
          list2 = {info.list2}
          list3 = {info.list3}/>, document.getElementById('myReactCode')
        );
      </script>
   </body>
 
 </html>