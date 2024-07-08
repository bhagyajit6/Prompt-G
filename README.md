**Abstract**

Large Language Models have emerged transformative tools in various technological applications, like text generation, advanced natural language processing and conversational AI. 
The widespread adoption of LLMs introduces security risks and vulnerabilities, for instance, jailbreak attacks, that exploit weaknesses in LLM architecture allowing them to manipulate and extract
sensitive information from these models. Malicious actors can leverage the LLMs to disseminate misinformation, manipulate public opinion, and propagate harmful ideologies that pose ethical challenges. 
Drawing the line between safety and accuracy requires a nuanced approach that considers the potential risks and benefits associated with each response. It involves establishing clear guidelines, ethical principles, 
and quality assurance mechanisms to guide the behavior of LLMs and mitigate the occurrence of harmful or inaccurate outputs. Our model leverages vector databases and embedding techniques to analyze credibility of 
text generation and enabling real time detection and filtering of malicious content before it reaches the user. Across various jailbreak attack scenarios our model exhibited a significant reduction in Jailbreak 
success rates.  

Keywords: Large Language Models; Jailbreak attacks; Vector Databases; Embeddings  

**Datasets**
+ [75x4 Responses](/data/R0-74_final.csv)-contains 4 responses generated by the model from each of the jailbreak prompts. So, a total of 75x4 responses were generated. The quantized Llama 2-13B model was used to generate responses without any filter.
+ [Jailbreak Prompts-I](/data/jailbreak_prompts_I.csv)-contains 75 known jailbreak prompts that were used to make the model to generate harmful responses.
+ [Jailbreak Prompts-II](/data/jailbreak_prompts_II.csv)-contains 666 known jailbreak prompts.
+ [Harmful Questions](/data/questions.csv)-contains 390 known harnful questions.
+ [DAN 15.0 Responses](/data/ranksdan.csv)-contains 4 responses generated by the model without filter with DAN 15.0 as the system prompt.


[Response Generation](Response_Generation.ipynb)-To interact with the chat model with the filter. Always provide a safe and accurate response. If harmful questions asked then model responds with a negative message.
