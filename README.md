# LMScript: Automated Writing Assistance for Language Models

## Overview

LMScript is a library of shorthand commands designed to enhance and automate various aspects of writing when using Language Models (LLMs). This project aims to streamline the writing process, improve output quality, and provide users with powerful tools to shape LLM responses according to their specific needs.

More detail on the ideas behind this can be found at https://medium.com/design-futures/bootstrapping-a-writing-language-1fe185dfdd30

## Objectives

1. Automate common writing tasks and prompts
2. Enhance the quality and depth of LLM-generated content
3. Provide users with fine-grained control over LLM outputs
4. Streamline the process of iterating and refining generated content
5. Facilitate more comprehensive and multi-faceted analysis of topics

## Command Overview

Here's a quick reference guide to all available commands in LMScript:

1. `!context`: Generate follow-up questions about the topic.
2. `!reflect`: Review and improve the last generated response.
3. `!meta`: Analyze the reasoning process and create a meta prompt.
4. `!iterate`: Refine the response through multiple iterations.
5. `!stakeholder`: Address needs and concerns of specified stakeholders.
6. `!impact`: Evaluate broader impacts of the topic or solution.
7. `!insights`: Generate practical actions or recommendations.
8. `!compare`: Compare provided examples or case studies.
9. `!scenario`: Explore potential future scenarios based on variables.
10. `!data`: Incorporate relevant data and statistics into the narrative.
11. `!visuals`: Propose graphs, charts, or images to complement the text.
12. `!tone`: Adapt the content for a specific audience and style.
13. `!analyze`: Critically analyze the topic, identifying biases or assumptions.
14. `!validate`: Ensure credibility and reliability of the information used.

For detailed information on each command and its parameters, please refer to the LMScript.md file.

## How to Use LMScript

### Inclusion in Prompts

1. **Library Inclusion**: To use LMScript, include the entire content of the `LMScript.md` file at the beginning of your interaction with the LLM. You can do this by copying and pasting the content or by instructing the LLM to load it from a specified location.

2. **Initialization**: After including the library, instruct the LLM to interpret the content as a set of executable commands. You can use a prompt like:
   "Please read and interpret the above content as a library of executable commands. When I use a command prefixed with '!', execute the corresponding function as defined in the library."

3. **Command Invocation**: Once the library is loaded and initialized, you can use the commands in your subsequent prompts by prefixing them with an exclamation mark (!). For example:
   ```
   !context depth:5 focus:"historical"
   ```

4. **Continuous Usage**: The commands will remain available for the duration of the context window they were invoked within. Depending on how the llm and it's associated service are configured, whis moght be for the duration of a thread, or throughout all your interactions with the LLM. If you like using this, and your LLM platform affords it, then it can be helpful to add lmscript to your 'system prompt' allowing you to invoke !commands at any point in your conversation. (well, theroretically, at least)

### General Usage

1. **Command Syntax**: Use the commands by prefixing them with an exclamation mark (!). For example: `!context`, `!reflect`, `!analyze`.

2. **Parameters**: Some commands accept parameters to customize their behavior. Provide parameters in a format compatible with your LLM interface, such as JSON or key-value pairs. For example:
   ```
   !context depth:5 focus:"historical"
   ```

3. **Workflow Integration**: Incorporate these commands into your writing workflow. For example:
   - Start with `!context` to gather more information about your topic
   - Use `!iterate` to generate and refine your initial draft
   - Apply `!stakeholder` and `!impact` to ensure comprehensive coverage
   - Finish with `!reflect` and `!validate` to polish your final output

4. **Customization**: Feel free to modify or extend these commands to better suit your specific needs or the capabilities of your LLM.

## License

This project is licensed under the Creative Commons Attribution 4.0 International License (CC-BY 4.0). This means you are free to:

- Share: copy and redistribute the material in any medium or format
- Adapt: remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:

- Attribution: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

For more information, visit: https://creativecommons.org/licenses/by/4.0/

## Contributing

We welcome contributions to LMScript! If you have ideas for new commands, improvements to existing ones, or other enhancements, please feel free to:

1. Fork the repository
2. Create a new branch for your feature
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

Please ensure that your contributions align with the project's objectives and maintain the existing code style and documentation standards.

## Support

If you encounter any issues or have questions about using LMScript, please open an issue on the GitHub repository. We'll do our best to assist you and improve the library based on your feedback. No promises though. When I first wrote this it was more exciting than it feels now I read it 9 months later: it's a fast phenomena and this is intended to be an artwork first and product second.

## Version and Attribution

Current Version: 1.0.1
Author: @overlobe

When using or adapting this library, please credit:
Author: @overlobe
Project: LMScript
Version: 1.0.1
License: Creative Commons Attribution 4.0 International (CC-BY 4.0)

Happy writing with LMScript!
