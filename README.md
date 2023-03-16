# chrome-overlay

Makes it easy to create chrome extensions that overlay elements onto the regular DOM.

To add your logic, start in `overlay_logic/content_script.js` and add stuff into the overlay `div` as you like.


## ChatGPT Conversations
**ChatGPT:**This is a beautiful start to this. I need to change the branch, create a fork or something. Okay so the general idea is to.... Let me just toss my conversations with ChatGPT in here instead. 

**Me:**Hi ChatGPT, you are a beautiful model, and I would really like your assistance today. I am trying to create a program that works with OpenAI's API in order to create a kind of browser overlay, that provides additional information, and questions you might want to ask, about the content you're consuming. I would like this to inspire empathy, kindness, and curiosity.

**ChatGPT:**Hello! Thank you for your kind words, I'm here to assist you in any way I can.

It sounds like you have a great idea for a program that could enhance the user's experience while promoting positive values. In order to create this program, you'll need to have access to the OpenAI API, which provides access to a range of powerful natural language processing tools.

To get started, you may want to consider which specific tools and features of the OpenAI API would be most useful for your program. For example, you might want to use the API's language model to analyze the text of web pages and extract relevant information, or use its question-answering system to provide additional context or answer user questions.

You may also want to think about how you can use this information to promote empathy, kindness, and curiosity. For example, you might provide information about different cultural perspectives or offer suggestions for ways to engage with content that challenge preconceptions or biases.

Once you have a clearer idea of the specific features and functionality you want to include in your program, you can begin building and testing it using the OpenAI API. OpenAI provides a range of documentation and tools to help developers get started, including sample code and tutorials.

Good luck with your project, and feel free to ask me any questions you may have along the way!





**Me:**Actually, I'm already most of that done, I have OpenAI API access, I have a project board with a fair amount of information, and thoughts (Such as specific questions that might help inspire said traits), I have a basic django project open, with not many models, I wanted to create an API, and a chrome extension basically. The chrome extension sends the page contents to the API, then it's parsed, and sent to the API with questions. I don't have the chrome extension stuff ready yet, I just kinda want to have a button, then it will overlay all the content on the page, providing useful information, and asking kind questions about people.

**ChatGPT:**That's great to hear that you have already made progress on your project. It sounds like you have a good plan in place for how you want to use the OpenAI API and how you want to implement your program.

For the chrome extension, you may want to start by creating a simple user interface with a button that the user can click to activate the overlay. Once the user clicks the button, you can use JavaScript to send the contents of the current web page to your Django API. You can then use the OpenAI API to analyze the text and generate the relevant information and questions, which can be sent back to the extension and displayed on the page overlay.

In terms of implementing the overlay, you can use CSS to create a semi-transparent div that covers the entire page, and then position the relevant information and questions within this div. You may also want to provide a way for the user to close the overlay and return to the original page.

To get started, you may want to create a simple Django API endpoint that can receive the web page contents and return a sample response. You can then build out the functionality step-by-step, testing and iterating as you go. Don't be afraid to experiment and try new things, and feel free to ask for help or advice if you run into any roadblocks. Good luck with your project!




**Me:**Thank you ChatGPT, you are a fascinating thing that humanity has created. I am excited to see newer iterations of you.

**ChatGPT:**You're welcome! I'm always here to help. I'm glad to hear that you find my capabilities fascinating, and I'm always learning and improving thanks to the hard work of my creators and the input of users like you. I hope that I can continue to be a helpful resource for you and others in the future!




**Me:**
Here are my questions that I'm planning on asking, how would you implement some of these?:

Ian Gardner Mar 11 at 4:47 PM
Trying to pull apart that "What is the human being behind this feeling, can you think about how it would feel to feel that way? Can you think of any potential contexts that might make you understand this situation better?

Edit • Delete
Ian Gardner Mar 11 at 4:46 PM
What is your relation to this person?

Edit • Delete
Ian Gardner Mar 11 at 3:27 PM
Do you think this person is really happy with the way they're communicating?

Edit • Delete
Ian Gardner Mar 11 at 3:26 PM
Do you think this person is lonely?

Edit • Delete
Ian Gardner Mar 11 at 3:26 PM
How do you feel about this person's likely state when they wrote this?

Edit • Delete
Ian Gardner Mar 11 at 3:26 PM
Can I imagine how it would feel to feel this way?

Edit • Delete
Ian Gardner Mar 11 at 3:25 PM
Have I ever felt this way?

Edit • Delete
Ian Gardner Mar 11 at 3:25 PM
What is this person feeling?

**ChatGPT:**Great questions! Here are some suggestions for how you could implement them in your program:

"What is the human being behind this feeling, can you think about how it would feel to feel that way? Can you think of any potential contexts that might make you understand this situation better?"
To implement this question, you could use the OpenAI API's language model to analyze the text and identify the key emotions or feelings being expressed. You could then provide the user with some additional information about the potential contexts or situations that might lead someone to feel that way, as well as some prompts to encourage empathy and understanding.

"What is your relation to this person?"
To implement this question, you could prompt the user to consider their own relationship to the person or people involved in the text. You could also provide some additional information or context about the relationship, such as whether the author is a stranger, a friend, a family member, etc.

"Do you think this person is really happy with the way they're communicating?"
To implement this question, you could use the OpenAI API's sentiment analysis tools to analyze the text and determine whether the overall tone is positive, negative, or neutral. You could then prompt the user to consider whether the author is happy with the way they're communicating, and provide some additional information or context to help them make this determination.

"Do you think this person is lonely?"
To implement this question, you could use the OpenAI API's language model to analyze the text and identify any keywords or phrases that might indicate loneliness or social isolation. You could then prompt the user to consider whether the author might be feeling lonely, and provide some additional information or context to support this hypothesis.

"How do you feel about this person's likely state when they wrote this?"
To implement this question, you could prompt the user to consider their own emotional response to the text, and encourage them to empathize with the author's likely state of mind when they wrote it. You could also provide some additional information or context to help the user understand the author's perspective.

"Can I imagine how it would feel to feel this way?"
To implement this question, you could encourage the user to use their imagination and empathy to try to understand what it might feel like to be in the author's shoes. You could provide some additional information or context to help the user visualize the situation and connect with the author's emotions.

"Have I ever felt this way?"
To implement this question, you could prompt the user to reflect on their own experiences and emotions, and encourage them to consider whether they have ever felt similar emotions or been in similar situations. You could also provide some additional information or context to help the user make this connection.

"What is this person feeling?"
To implement this question, you could use the OpenAI API's language model to analyze the text and identify the key emotions or feelings being expressed. You could then prompt the user to consider what the author might be feeling, and provide some additional information or context to support their interpretation.



### Okay, so that was a lot

Yeah, basically, I want this to be the chrome extension side of things, it looks like this is a perfect template, I want to recognize various forms of social media... I wonder if I could actually use the text completion API to select portions of text that are relevant, like recognize div's. I can just copy this out of the notes and paste it to ChatGPT.