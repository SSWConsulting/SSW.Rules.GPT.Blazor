<a href="https://www.ssw.com.au">
  <img src="https://raw.githubusercontent.com/SSWConsulting/SSW.Rules.Content/main/_docs/images/ssw-banner.png">
</a>

> **Note**  
> This readme was generated by SSW Rules GPT

# SSW Rules GPT 🤖

### 📝 Project Description

Our project is a GPT Bot that uses OpenAI embeddings to search for matching [SSW Rules](https://www.ssw.com.au/rules), and then feeding the top 10 results back into the ChatGPT API, written in C# and Blazor.

### 💻 Installation

Follow these simple steps to install and set up our SSW Rules GPT project:

1. Clone the repository
2. Add the following to your secrets.json file in `src/WebAPI`:
```
{
  "OpenAiApiKey": "{{ OPENAI API KEY }}",
  "ConnectionStrings": {
    "DefaultConnection": "{{ DATABASE CONNECTION STRING }}"
  }
}
```

> **Note**  
> You can find the key and connection string in Keeper

3. Run the WebAPI (https) project
4. Run the WebUI project, and a browser window will open to https://localhost:5002
   
> **Warning**  
> The RulesGPT frontend has been changed from port 5001 to 5002, if you are running Identity Server locally you **must** be running on port 5002.  
> Double check WebUI/launchsettings.json before running the project.

5. Ask SSW Rules GPT a question!

### 💻 Installation - Set Multiple Startup Projects
Instead of manually launching the WebUI and WebAPI projects, you can set multiple startup projects in Visual Studio and Rider.  
Read [this rule](https://ssw.com.au/rules/multiple-startup-projects/) to learn how.

### 🚀 Deployment
When code merged into main it will be automatically deployed to staging.
You should test your changes in staging before manually running the production workflow.

Staging Frontend URL: https://ashy-meadow-0a2bad900.3.azurestaticapps.net  
Staging API URL: https://ssw-rulesgpt-api-stage.azurewebsites.net

### 👥 Project Contributors

- Calum Simpson ([@calumjs](https://github.com/calumjs))
- Matt Parker ([@MattParkerDev](https://github.com/MattParkerDev))
- Harry Ross ([@Harry-Ross](https://github.com/Harry-Ross))
- Jack Reimers ([@jackreimers](https://github.com/jackreimers))
- Adam Cogan ([@adamcogan](https://github.com/adamcogan))
