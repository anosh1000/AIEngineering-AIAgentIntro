Interactive chatbot UI using a ReAct AI Agent with openAI automated function calls
If the user asks "What are some fun activities to do?", the agent will decide it needs to run the function getLocation(), then it will decide it needs to run getCurrentWeather() passing in the location as the argument. Then, it will decide it has enough information to answer the user's question and will output a thoughtful response based off the system prompt.
<pre>
  Topics Covered
  ReAct Agent - Allowing openai API to decide which function(s) to call. Use output of function(s) in final response back to user
  Main idea of ReAct Agents is the looping of calling functions until agent decides it has enough information to answer user
  Old way of automating function calls used Regex, tool_calls, looping, max_iterations, pushing function outputs to messages array, and creating object of function names to find the function based off the string containing the function name passed by the agent. 
  Now, openai.chat.completions.runTools automates the process.
</pre>
