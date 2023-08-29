# AIVA
GPT-3.5 Turbo Based Virtual Agent that provides replies with user-provided data via PDF files

AIVA has an adjacent folder called trainingDocs. This folder contains pdf files which serve as the training
material. They can be anything from an HR manual to sample resumes, to even studies on the heart
anatomy.

In summary, this code creates a web-based chatbot interface using Gradio and utilizes the GPT-3.5
language model through the OpenAI API to provide intelligent responses to user queries. The index is
constructed to optimize response retrieval from the provided training documents.

‘construct_index’ function: This function constructs a GPT-like index using the provided
training documents stored in a given directory. The documents will be indexed to efficiently
retrieve responses from the chatbot.

‘chatbot’ function: This function takes an input text (user query) and queries the GPT-like
index constructed earlier. It uses the GPTSimpleVectorIndex to retrieve a response from the
indexed documents based on the input text.

Gradio Interface setup: An instance of the Gradio Interface is created with the function
chatbot as the core chatbot logic. The interface accepts user input through a textbox,
allowing the user to enter their query. The output is displayed as text, showing the chatbot&#39;s
response. The interface is titled &quot;AIVA.&quot;

Index construction and interface launch: The ‘construct_index’ function is called to build
the GPT-like index using training documents found in the &quot;trainingDocs&quot; directory. The index
is then saved to disk in JSON format. The Gradio interface is launched, making the chatbot
accessible through a web browser. The share=True parameter allows the interface to be
shared publicly.
