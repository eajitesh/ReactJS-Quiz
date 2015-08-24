# ReactJS-Quiz
This is a quiz framework created using ReactJS. 

Following is a sample JSON data model which could be posted to create the quiz:
```json
var test = {
		name: "Sample Test",
		description: "This is a sample test paper to demonstrate the ReactJS UI design by components.",
		passCutoff: 0.33,		
		applyNegativeMarking: false,
		questions: [
			{
			no: "1",
			qtext:"California is in which part of USA?",
			options:[
				{text:"East"},
				{text:"Mid"},
				{text:"West"},
				{text:"South"}
			],
			ans:"West",
			marks: 3
		},
		{
			no: "2", 
			qtext:"Who is the Prime Minister of India?",
			options:[
				{text:"Sonia Gandhi"},
				{text:"Narendra Modi"},
				{text:"Manmohan Singh"},
				{text:"Rahul Gandhi"}
			],
			ans:"Narendra Modi",
			marks: 2
		},
		{
			no: "3",
			qtext:"Which of the following is most popular Search Engine Company?",
			options:[
				{text:"Microsoft"},
				{text:"Facebook"},
				{text:"Google"},
				{text:"Yahoo"}
			],
			ans:"Google",
			marks: 1
		},
		]
	};	
```	
The above Test JSON object could then be passed to Test Component like following:
	
React.render( &lt;Test details={test}/&gt;, document.getElementById( "content" ) );
