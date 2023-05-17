## PKG ontology description

PKG ontology is proposed to create personal knowledge graphs for web search. It was implemented in OWL using the Protégé editor. This resource fills the need 
for semantic representation of the user's profile and data related search activity under a unified framework that accommodates associations between entities and attributes.
Our ontology introduces the necessary classes and properties to construct a Personal Knowledge Graph on a web search environment. 

PKG ontology extends on the EduCOR (educor) ontology[^1] and reuses syntax for its classes and properties from schema.org[^2] (schema), and friend of a friend vocabulary[^3] (foaf).

Our ontology is aligned with FAIR principles[^4]. Our data and metadata are assigned globally unique and persistent identifiers and clearly and explicitly include the
identifier of the data they describe. They are described in rich metadata, and we reuse vocabularies that follow FAIR principles and include qualified references to them.
Our ontology will be found in a public registry, which also offers the full documentation and visualisation of the ontology. The ontology data can be retrieved 
from there via the querying API. 
Also, we describe the scope of our data and have them published under the licence CC BY-SA 4.0.

The main class in our ontology is the *SearchSession* as it is also highlighted in the Figure:

![PKG ontology](https://github.com/tibonto/pkg/raw/gh-pages/Pkgonto.png)

Together with the classes *UserProfile*, and *Group* they create the *InputStream* for the computational algorithm that will perform the semantic annotation. The ontology can be used to 
create a Personal Knowledge Graph and enhance semantically a back end of a web search application, when linking to knowledge graphs. That can happen via the 
*RecognizedEntites* which returns the output result of the computation of the connection with Linked Open Data resources. The result is the recognized entities 
from the connected knowledge graph together with their confidence score based on the named entity recognition software that is utilised. Finally, the *SharedObject* 
shares the items needed for the downstream application related to search activity with respect to user's privacy and accessibility rights from the *Accessibility* class.

The goal of next generation KGs is to create more intelligent and responsive systems that can better support a wide range of applications, including semantic search, and intelligent personal assistants. These systems have the potential to revolutionize the way we interact with data and information, and may play an increasingly important role in fields such as artificial intelligence and data science. Having as a goal to address some of the limitations of current knowledge graphs, we aim to create the basis for more sophisticated reasoning capabilities and explainability. To accommodate this demand we define the classes *InputStream* and *SharedObject* which record the entities shared with external resources. Furthermore, we record the timestamp and author metadata for actions that require algorithmic personalisation, and the confidence score of each recognised entity.

[^1]: Ilkou, E., Abu-Rasheed, H., Tavakoli, M., Hakimov, S., Kismihók, G., Auer, S., Nejdl, W.: Educor: An educational and career-oriented recommendation ontology.
In: International Semantic Web Conference. pp. 546–562. Springer (2021)
[^2]: https://schema.org/
[^3]: http://xmlns.com/foaf/spec/
[^4]: Wilkinson, M.D., Dumontier, M., Aalbersberg, I.J., Appleton, G., Axton, M., Baak, A., Blomberg, N., Boiten, J.W., da Silva Santos, L.B., Bourne, P.E., et al.: The fair
guiding principles for scientific data management and stewardship. Scientific data 3(1), 1–9 (2016)
