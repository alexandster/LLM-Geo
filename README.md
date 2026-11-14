# Autonomous GIS: the next-generation AI-powered GIS
- This repository was forked from https://github.com/gladcolor/LLM-Geo   

# Installation

Clone or download the repository, rename `your_config.ini` as `config.ini`. Then, put your OpenAI API key in the `config.ini` file. Please use GPT-4 or higher, the lower versions such as 3.5 do no have enough reasoning ability to generate correct solution graph and operation code. 

# How to use
- Download all files, put your question to the `TASK` variable in LLM_Geo_API4.ipynb.
- Set the `task_name` in the notebook. Space is not allowed. LLM-Geo will create the fold using the `task_name` to save results.
- Run all cells.
- LLM-Geo will use the backed LLM (GPT-4 now) to review and debug the generated program. GPT-4's debugging ability is still weak. The default maximum attempt count is set to 10; modify this value is needed. 
- Note that the solution based on graph, code review, and debug will cost a lot of tokens. We provide a Jupyter notebook [(Direct_request_LLM.ipynb)](https://github.com/gladcolor/LLM-Geo/blob/master/Direct_request_LLM.ipynb) to directly request solutions from LLM. This is a much more quick way to get solutions for simple tasks/questions, but its robustness may be slightly lower.

# Note:

- You may need the [geopandas](https://geopandas.org/en/stable/getting_started.html#installation) package to load vector files. Please install it in advance.

# Other relevant projects:
- Geodata Retriever Agent:
  - [QGIS plugin](https://github.com/Teakinboyewa/AutonomousGIS_GeodataRetrieverAgent)
  - [Code](https://github.com/gladcolor/LLM-Find/)
- Spatial Analysis Agent:
  - [QGIS Plugin](https://plugins.qgis.org/plugins/SpatialAnalysisAgent-master/#plugin-versions) 
  - [Code](https://github.com/Teakinboyewa/SpatialAnalysisAgent)

# Literature
- Zhenlong Li & Huan Ning (2023) Autonomous GIS: the nextgeneration AI-powered GIS, International Journal of Digital Earth, 16:2, 4668-4686, DOI: [10.1080/17538947.2023.2278895](https://doi.org/10.1080/17538947.2023.2278895)
- Ali Khosravi Kazazi , Zhenlong Li, M. Naser Lessani & Guido Cervone (2026) From questions to queries: an AI-powered multi-agent framework for spatial text-to-Sql, International Journal of Digital Earth, 19:2, 2687193, DOI: [10.1080/17538947.2026.2687193](https://doi.org/10.1080/17538947.2026.2687193)
- Ali Khosravi Kazazi & Zhenlong Li (2026) From tool to collaborator: rethinking GIScience as GIS becomes agentic and autonomous, International Journal of Digital Earth, 19:1, 2687228, DOI: [10.1080/17538947.2026.2687228](https://doi.org/10.1080/17538947.2026.2687228)
- Zhenlong Li , Ali Khosravi Kazazi , Ruixiang Liu , Temitope Akinboyewa , Huan Ning , Xiao Huang , Xinyue Ye , Samantha T. Arundel , Wenwen Li , Chaowei Yang , Shaowen Wang & Ingo Simonis (2026) Geospatial Agentic Services: a framework for interoperable geospatial intelligence, Annals of GIS, ahead-of-print:ahead-of-print, 1-21, DOI: [10.1080/19475683.2026.2738374](https://doi.org/10.1080/19475683.2026.2738374)
- Temitope Akinboyewa, Zhenlong Li, Huan Ning & M. Naser Lessani (2025) GIS Copilot: towards an autonomous GIS agent for spatial analysis, International Journal of Digital Earth, 18:1, 2497489, DOI: [10.1080/17538947.2025.2497489](https://doi.org/10.1080/17538947.2025.2497489)
- Ruixiang Liu , Zhenlong Li & Ali Khosravi Kazazi (2026): Towards intelligent geospatial data discovery: a knowledge graph-driven multi-agent framework
powered by large language models, International Journal of Geographical Information Science, DOI: [10.1080/13658816.2026.2724505](https://doi.org/10.1080/13658816.2026.2724505)
- Zhenlong Li, Huan Ning, Song Gao, Krzysztof Janowicz, Wenwen Li, Samantha T. Arundel, Chaowei Yang, Budhendra Bhaduri, Shaowen Wang, A-Xing Zhu, Mark Gahegan, Shashi Shekhar, Xinyue Ye, Grant McKenzie, Guido Cervone & Michael E. Hodgson (2025) GIScience in the era of Artificial Intelligence: a research agenda towards Autonomous GIS, Annals of GIS, 31:4, 501-536, DOI: [10.1080/19475683.2025.2552161](https://doi.org/10.1080/19475683.2025.2552161)


