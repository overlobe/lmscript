# LMScript Command Library

Version: 1.0.0
Author: @overlobe
License: CC-BY 4.0

This document defines a set of executable commands for Language Models (LLMs). When a command is invoked with an exclamation mark (!), execute the corresponding function.

## Version History

- 1.0.0: Initial release with 14 core commands

## Command Definitions

1. !context(depth: int = 3, focus: str = None)
   Function: Generate 'depth' number of follow-up questions about the topic. If 'focus' is specified, tailor questions to that aspect.

2. !reflect(criteria: str = None)
   Function: Review the last generated response. Identify areas for improvement based on 'criteria' if specified. Generate and return a revised version.

3. !meta()
   Function: Analyze your own reasoning process for the last response. Label the steps in your chain of thought. Create and return a meta prompt to enhance the next response.

4. !iterate(iterations: int = 3, focus: str = None)
   Function: Generate an initial response to the last prompt. Then, perform 'iterations' number of refinements, focusing on 'focus' aspect if specified. Return the final iteration.

5. !stakeholder(stakeholders: list)
   Function: Ensure the last generated content addresses the needs and concerns of each stakeholder in the 'stakeholders' list. Return an updated version of the content.

6. !impact(timeframe: str = "long-term", domains: list = ["social", "environmental", "economic"])
   Function: Evaluate the broader impacts of the last discussed topic or solution. Consider the specified 'timeframe' and 'domains'. Return a comprehensive impact analysis.

7. !insights(count: int = 3, type: str = "strategic")
   Function: Based on the last analysis or discussion, generate 'count' number of practical actions or recommendations of the specified 'type'. Return these insights.

8. !compare(examples: list, aspects: list = None)
   Function: Compare the 'examples' provided, highlighting similarities and differences. If 'aspects' are specified, focus the comparison on these aspects. Return a detailed comparison.

9. !scenario(variables: list, timeframe: str = "5 years")
   Function: Explore potential future scenarios based on the 'variables' provided, considering the specified 'timeframe'. Return a description of possible outcomes.

10. !data(source: str = None, type: str = "mixed")
    Function: Incorporate relevant data and statistics into the narrative. Use the specified 'source' if provided, and focus on the 'type' of data requested. Return the enhanced content.

11. !visuals(type: str = "graph", count: int = 1)
    Function: Propose 'count' number of 'type' visuals that could complement the text. Return descriptions of these visuals.

12. !tone(audience: str, style: str = "formal")
    Function: Rewrite the last generated content to suit the specified 'audience' using the requested 'style'. Return the adapted content.

13. !analyze(depth: str = "in-depth", focus: list = None)
    Function: Critically analyze the last topic discussed. Use the specified 'depth' of analysis and focus on the aspects in 'focus' if provided. Identify potential biases or assumptions. Return the analysis.

14. !validate(criteria: list = ["source credibility", "methodology"], level: str = "thorough")
    Function: Assess the credibility and reliability of the information used in the last response. Apply the specified 'criteria' at the requested 'level'. Return a validation report.

## Execution Instructions

1. When a command is invoked with an exclamation mark (!), execute the corresponding function.
2. Use default parameter values if not explicitly provided in the command.
3. Return the result of the command execution as your next response.
4. If a command is not recognized, inform the user and provide the list of available commands.

## Attribution

When using or adapting this library, please credit:

Author: @overlobe

Project: LMScript

Version: 1.0.0

License: Creative Commons Attribution 4.0 International (CC-BY 4.0)
