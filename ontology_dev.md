## Ontology Development

Following ontology development guidelines[^1], we initially define the domain and scope of our ontology which is the support and basis of PKGs creation and population in a web search environment. We define our competency questions as follows:
• Which parameters determine the personalisation?
• How is the connection with external Knowledge Graphs and Linked Open Data resources supported?
• How is the user's privacy maintained?
Following our scope, we perform a literature review on resources related to user profiling, user modeling and web search. From our audit, we decide to reuse parts from the https://schema.org/ and http://xmlns.com/foaf/0.1/ vocabularies, and https://tibonto.github.io/educor/ ontology. From the latter we adapt the user profile pattern to the web search use case.
Next we determined the main classes in our ontology, and a class hierarchy which defines the snippet and webpage as subclasses of class related to  search results, and search session as a subclass of the class *UserLogs* of the high ontology EduCOR[^2], and finally we set the cardinality and instances of our ontology.

[^1]: Noy, N.F., McGuinness, D.L., et al.: Ontology development 101: A guide to creating your first ontology (2001)
[^2]: Ilkou, E., Abu-Rasheed, H., Tavakoli, M., Hakimov, S., Kismihók, G., Auer, S., Nejdl, W.: Educor: An educational and career-oriented recommendation ontology. In: International Semantic Web Conference. pp. 546–562. Springer (2021)
