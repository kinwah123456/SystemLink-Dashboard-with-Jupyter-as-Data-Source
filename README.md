# SystemLink-Dashboard-with-Jupyter-as-Data-Source

This repo contains sample Jupyter Notebook code that can be used to receive parameter(s) from the SystemLink Dashboard and provide outputs to the SystemLink Dashboard.
The working principle will be covered below.

<img width="1701" height="859" alt="image" src="https://github.com/user-attachments/assets/bcdc18e8-80a1-4469-91cf-9bf1d5b09270" />



Example #1
Output Correctly.ipynb             -> To display static 50 in both Numeric Tile and Progress Tile.

Example #2
Output Correctly with Input.ipynb  -> To receive a numeric parameter and display it in both Numeric Tile and Progress Tile.

Both Example #1 and Example #2 will display a static bar graph if Graph Tile is selected.

## Working Principle
1. Import scrapbook as sb. We will be using scrapbook to output data to the SystemLink Dashboard.
2. On the right sidebar, open the Property Inspector pane.
<img width="1708" height="960" alt="image" src="https://github.com/user-attachments/assets/cad3c44e-c1ee-4ef0-8991-1b2280efee45" />

3. Update Cell Metadata by adding the parameters, the parameter default values, and the outputs.
4. Ensure the output you would like to display at SystemLink Dashboard is structured correctly as shown by the *result* variable
5. Record results with Scrapbook by using the following code: sb.glue('result', result)

## Useful References
1. [Creating a New Jupyter Notebook](https://www.ni.com/docs/en-US/bundle/systemlink-server/page/creating-a-new-jupyter-notebook.html)
2. [Pass Inputs Into a SystemLink Jupyter Notebook](https://knowledge.ni.com/KnowledgeArticleDetails?id=kA0VU0000000giP0AQ&l=en-MY)
3. [Configure Multiple Outputs in SystemLink Jupyter Notebook](https://knowledge.ni.com/KnowledgeArticleDetails?id=kA0VU0000000dnl0AA&l=en-MY)
