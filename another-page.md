---
layout: default
---

# METHODOLOGY
>
## PROMPTING TECHNIQUES

The LLMS used were: CHAT GPT, LLAMA,  GEMINI.

**The prompting techniques used were Zero-shot Prompting, Few-Shot Prompting, Chain-of-thought, and Generated-knowledge-prompting. To enrich the knowledge graph we asked the following questions:**
1. Enhance the "a-cd:subject" Relationship
Cultural Property: Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)
Owner: Damiano Chiesa
What are the craftsmanship techniques used in the 'Cappotto, maschile – Novità Confezioni Italiane Eleganza'?
Take into account that Craftsmanship is the skill that someone uses when they make beautiful things with their hands. 
2. Can you extract exactly what the main topics are based on this answer? 
3. Could you transform this description into RDF format? Explain the process for getting this RDF format. 
4. Could you use the ArCo clothing ontology? 







## Enhance the "a-cd:subject" Relationship
Cultural Property: Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)
Owner: Damiano Chiesa

**What are the craftsmanship techniques used in the 'Cappotto, maschile – Novità Confezioni Italiane Eleganza'?**
Take into account that Craftsmanship is the skill that someone uses when they make beautiful things with their hands.

**- Chat GPT**

The craftsmanship techniques used in the 'Cappotto, maschile – Novità Confezioni Italiane Eleganza' can vary depending on the specific details and construction of the coat. However, here are some common craftsmanship techniques that may be employed:

1. Tailoring: This involves the precise cutting and sewing of fabric to create a garment that fits well and has clean lines. Tailoring techniques may include hand-sewing, machine sewing, and pattern drafting.

2. Stitching: Various types of stitching may be used in the construction of the coat, including hand stitches like backstitch, slip stitch, and blind hem stitch, as well as machine stitches like straight stitch and zigzag stitch.

3. Detailing: Craftsmanship often involves intricate detailing to enhance the aesthetic appeal of the garment. This may include decorative stitching, embroidery, appliqué, or embellishments like buttons, beads, or sequins.

4. Finishing: Finishing techniques are used to refine the appearance and durability of the coat. This may involve techniques such as seam finishing (e.g., serging, French seams), edge stitching, pressing, and hand-finishing details.

5. Fabric manipulation: Craftsmen may use various techniques to manipulate the fabric to achieve desired effects, such as pleating, gathering, tucking, or draping.

6. Handwork: Many high-quality garments feature handwork, where skilled artisans perform tasks that cannot be replicated by machines. This may include hand-rolled hems, hand-sewn buttonholes, hand-applied trims, or hand-beading.

These are just a few examples of the craftsmanship techniques that could be used in the creation of the 'Cappotto, maschile – Novità Confezioni Italiane Eleganza'. Each garment is unique, and the specific techniques employed may vary based on the designer's vision, the materials used, and the desired aesthetic and functionality of the coat.

- **LLAMA**

What a remarkable cultural property! The "Cappotto, maschile – Novità Confezioni Italiane Eleganza" (Male Coat – Italian Elegant Fashion Novelties) is a magnificent showcase of Italian craftsmanship, especially in tailoring. Let's explore some of the craftsmanship techniques employed in crafting this exquisite piece:

Cutting: The coat's pattern pieces were meticulously cut from premium fabrics like wool or cashmere using scissors or a rotary cutter. The precision of the cuts ensures a perfect fit and a sleek silhouette.

Sewing: Skilled seamstresses combined hand-stitching and machine-stitching techniques to sew the coat's seams. The evenness and consistency of the stitches create a strong bond between fabric pieces, ensuring durability.

Tailoring:The coat's design and construction exemplify the art of tailoring. Tailors expertly shape and fit the fabric to the body, crafting a comfortable and flattering silhouette. Attention to detail is evident in the padding, lining, and quilting.

Embroidery: Intricate embroidery embellishes the coat, showcasing the embroiderer's skill. Delicate stitches and patterns require patience and precision, resulting in exquisite artwork.

Finishing:Finishing techniques, including interlinings, facings, and buttons, highlight Italian craftsmanship. The coat's lining and padding add comfort and luxury to the design.

Quality Control: Rigorous quality control ensures the coat meets the highest standards. Inspection for defects underscores the commitment to excellence in craftsmanship.

The "Cappotto, maschile – Novità Confezioni Italiane Eleganza" is a masterpiece, epitomizing Italian craftsmanship. Its attention to detail, precision, and quality exemplify Italy's rich tradition of tailoring and fashion design.
    
- **GEMINI**

Here's how you can enhance the "a-cd:subject" relationship to describe potential craftsmanship techniques used in the "Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)" even though we don't have specific details:

Use a broader concept:
Instead of listing specific techniques (which we don't have), link the subject to a broader concept like "Men's Tailoring (20th Century)". This indicates that the coat was likely crafted using techniques typical of that period.
Include a reference description:
Create a separate RDF description that details these typical techniques. You can reference this description within the "a-cd:subject" relationship.
Here's the RDF snippet demonstrating this approach:
```rdf
<rdf:Description rdf:about="http://example.org/cappotto_maschile">
  <dc:title>Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)</dc:title>
  <arco:type rdf:resource="http://vocab.getty.edu/aat/300223001"/>  
  <arco:gender rdf:resource="http://vocab.getty.edu/aat/300100100"/>
  <f:owner rdf:resource="http://example.org/damiano_chiesa"/>  
  <f:productionPeriod rdf:datatype="http://www.w3.org/2001/XMLSchema#date">1901/01/01^^xsd:date</f:productionPeriod>
  <a-cd:subject rdf:resource="http://example.org/mens_tailoring_20th_century"/>
</rdf:Description>

<rdf:Description rdf:about="http://example.org/mens_tailoring_20th_century">
  <dc:title>Men's Tailoring Techniques (20th Century)</dc:title>
  <f:technique rdf:resource="http://vocab.getty.edu/aat/300131999"/>  <f:technique rdf:resource="http://vocab.getty.edu/aat/300132010"/>  </rdf:Description>
```
Explanation:

The first description for the coat ([http://example.org/cappotto_maschile](http://example.org/cappotto_maschile)) links the subject to the broader concept "Men's Tailoring (20th Century)" using the `a-cd:subject` property with a reference to the second description's URI.
The second description ([http://example.org/mens_tailoring_20th_century](http://example.org/mens_tailoring_20th_century)) provides a title and lists potential techniques using the `f:technique` property with URIs from a relevant ontology (e.g., Getty AAT). You can add more techniques based on your research.

Benefits:

This approach acknowledges the lack of specific information about the coat's craftsmanship.
It provides context by linking to a description of typical techniques used during that period.
You can expand the reference description ([http://example.org/mens_tailoring_20th_century](http://example.org/mens_tailoring_20th_century)) to include additional details about these techniques over time.

Note:
Replace the example URIs with the actual URIs from the relevant ontologies.







## Can you extract exactly what the main topics are based on this answer?

**- Chat GPT**

  Sure, here are the main topics extracted from the answer:
1. Tailoring techniques
2. Stitching methods
3. Detailing and embellishments
4. Finishing techniques
5. Fabric manipulation
6. Handwork and artisanal techniques

**- LLAMA**

Based on the answer, the main topics are:
1. Cutting
2. Sewing
3. Tailoring
4. Embroidery
5. Finishing
6. Quality control
These topics relate to the craftsmanship techniques used in the creation of the "Cappotto, maschile – Novità Confezioni Italiane Eleganza" cultural property.

- **GEMINI**

The main topics covered in this answer are:
1. Cultural Property: Men's Coat (Cappotto, maschile)
2. Description: 
    Title: "Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)" (translates to "Men's Coat - New Italian Fashions Elegance (20th Century)")
    Owner: Damiano Chiesa
3. Missing Information: Specific craftsmanship techniques used for the coat.
4. Enhancing "a-cd:subject" Relationship: 
   Strategy:
       Use a broader concept: "Men's Tailoring (20th Century)" to indicate potential techniques.
       Include a separate reference description detailing these techniques (e.g., canvas construction, hand-stitching).
       Benefits:
         Acknowledges lack of specific details.
         Provides context with typical techniques of the period.





   

## Could you transform this description into RDF format? Explain the process for getting this RDF format.


- **Chat GPT**

To transform the given description into RDF format, we can use the RDF Schema (RDFS) vocabulary to define classes and properties, and then create RDF triples representing the data. Here's how we can do it:

1. Identify Entities and Properties:
   - Identify the entities (subjects) and properties (predicates) in the description. In this case, the main entities are the "Cappotto, maschile – Novità Confezioni Italiane Eleganza" and the craftsmanship techniques. The properties include the type of craftsmanship technique and its description.

2. Define Classes and Properties:
   - Use RDF Schema (RDFS) to define classes and properties. For example, we can define a class for "Cappotto, maschile – Novità Confezioni Italiane Eleganza" and properties for "craftsmanship technique" and "description".

3. Create RDF Triples:
   - Represent the data using RDF triples, where each triple consists of a subject, predicate, and object. For example, `<coat_uri> rdf:type :Coat .` indicates that the coat has the type "Coat".

Here's an example of how the description can be represented in RDF format:

```turtle
@prefix ex: <http://example.org/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

# Define classes
ex:Coat a rdfs:Class .
ex:CraftsmanshipTechnique a rdfs:Class .

# Define properties
ex:hasCraftsmanshipTechnique a rdf:Property ;
                            rdfs:domain ex:Coat ;
                            rdfs:range ex:CraftsmanshipTechnique .
ex:description a rdf:Property ;
               rdfs:domain ex:CraftsmanshipTechnique ;
               rdfs:range rdfs:Literal .

# Create instances and relationships
ex:Coat1 a ex:Coat ;
         ex:hasCraftsmanshipTechnique ex:Tailoring .

ex:Tailoring a ex:CraftsmanshipTechnique ;
              ex:description "Tailoring involves precise cutting and sewing of fabric..." .
```

In this RDF representation:
- We define classes for "Coat" and "CraftsmanshipTechnique".
- We define properties for "hasCraftsmanshipTechnique" and "description".
- We create an instance of the coat and a specific craftsmanship technique (Tailoring).
- We establish a relationship between the coat and the craftsmanship technique, and provide a description for the technique.

You can follow similar steps to represent other entities and properties from the description in RDF format.
 
- **LLAMA**
 
 To transform the description into RDF (Resource Description Framework) format, I'll follow these steps:
1. Identify the entities: Extract the main entities mentioned in the description, such as the cultural property, techniques, and materials.
2. Create RDF triples: Represent each entity as a subject-predicate-object triple, where the subject is the entity, the predicate is a property or relationship, and the object is the value or description of the entity.
3. Use standardized vocabularies: Utilize standardized vocabularies like Dublin Core (DC) for metadata and CIDOC CRM (Conceptual Reference Model) for cultural heritage information to ensure interoperability and reusability.
Here's the RDF representation of the description:
```rdf
@prefix dc: <http://purl.org/dc/elements/1.1/>.
@prefix cidoc: <http://www.cidoc-crm.org/cidoc-crm/>.
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
<http://example.org/CappottoMaschile> a cidoc:E55_Material_Manifestation ;
dc:title "Cappotto, maschile – Novità Confezioni Italiane Eleganza" ;
dc:description "A male coat created by Italian fashion designers, showcasing craftsmanship techniques.".
<http://example.org/Cutting> a cidoc:E55_Material_Manifestation ;
dc:title "Cutting" ;
rdfs:comment "The process of cutting fabric for the coat.".
<http://example.org/Sewing> a cidoc:E55_Material_Manifestation ;
dc:title "Sewing" ;
rdfs:comment "The process of stitching fabric pieces together for the coat.".
<http://example.org/Tailoring> a cidoc:E55_Material_Manifestation ;
dc:title "Tailoring" ;
rdfs:comment "The process of shaping and fitting fabric to create the coat's design.".
<http://example.org/Embroidery> a cidoc:E55_Material_Manifestation ;
dc:title "Embroidery" ;
rdfs:comment "The process of decorating the coat with intricate stitches and patterns.".
<http://example.org/Finishing> a cidoc:E55_Material_Manifestation ;
dc:title "Finishing" ;
rdfs:comment "The process of adding the final touches to the coat, such as interlinings, facings, and buttons.".
<http://example.org/QualityControl> a cidoc:E55_Material_Manifestation ;
dc:title "Quality Control" ;
rdfs:comment "The process of inspecting the coat for defects or imperfections.".
<http://example.org/CappottoMaschile> cidoc:P126_carries_content <http://example.org/Cutting>.
<http://example.org/CappottoMaschile> cidoc:P126_carries_content <http://example.org/Sewing>.
<http://example.org/CappottoMaschile> cidoc:P126_carries_content <http://example.org/Tailoring>.
<http://example.org/CappottoMaschile> cidoc:P126_carries_content <http://example.org/Embroidery>.
<http://example.org/CappottoMaschile> cidoc:P126_carries_content <http://example.org/Finishing>.
<http://example.org/CappottoMaschile> cidoc:P126_carries_content <http://example.org/QualityControl>.
```
In this RDF representation:
* `<http://example.org/CappottoMaschile>` is the URI for the cultural property, "Cappotto, maschile – Novità Confezioni Italiane Eleganza".
* The `dc:title` and `dc:description` properties provide
  
- **GEMINI**

 Absolutely! Here's the description transformed into RDF format using the approach we discussed:

Part 1: Description of the Coat

```rdf
<rdf:Description rdf:about="http://example.org/cappotto_maschile">
  <dc:title>Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)</dc:title>
  <arco:type rdf:resource="http://vocab.getty.edu/aat/300223001"/>  
  <arco:gender rdf:resource="http://vocab.getty.edu/aat/300100100"/>
  <f:owner rdf:resource="http://example.org/damiano_chiesa"/>  
  <f:productionPeriod rdf:datatype="http://www.w3.org/2001/XMLSchema#date">1901/01/01^^xsd:date</f:productionPeriod>
  <a-cd:subject rdf:resource="http://example.org/mens_tailoring_20th_century"/>
</rdf:Description>
```

Explanation (Part 1):

1. We define a resource for the coat (`http://example.org/cappotto_maschile`).
2. Title, type, gender, owner, and production period are described as before.
3. We use the `a-cd:subject` property to link to the reference description  using the URI `http://example.org/mens_tailoring_20th_century`.

**Part 2: Reference Description of Tailoring Techniques**

```rdf
<rdf:Description rdf:about="http://example.org/mens_tailoring_20th_century">
  <dc:title>Men's Tailoring Techniques (20th Century)</dc:title>
  <f:technique rdf:resource="http://vocab.getty.edu/aat/300131999"/>  <f:technique rdf:resource="http://vocab.getty.edu/aat/300132010"/>  </rdf:Description>
```

Explanation (Part 2):

1. We define a separate resource (`http://example.org/mens_tailoring_20th_century`) for the reference description.
2. The title indicates it describes tailoring techniques.
3. We use the `f:technique` property with URIs from a relevant ontology (e.g., Getty AAT) to specify potential techniques used during the 20th century.  

Process:

1. We first describe the coat itself using basic properties like title, type, etc.
2. We acknowledge the lack of specific details about craftsmanship techniques.
3. We create a separate resource to describe typical tailoring techniques of the relevant period.
4. We link the coat description to this reference description using the `a-cd:subject` property.

This approach provides a more comprehensive representation of the available information and the context for the coat.
      






## Could you use the ArCo clothing ontology?


- **Chat GBT**

Certainly! We can use the ArCo (Archivio dei beni culturali) ontology, which provides a standardized way to represent cultural heritage assets, including clothing items and related concepts. Here's how we can represent the given description using the ArCo ontology:

```turtle
@prefix arco: <http://w3id.org/arco/ontology/arco/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

# Define classes
arco:ClothingItem a rdfs:Class ;
                  rdfs:subClassOf arco:CulturalHeritageAsset .
arco:CraftsmanshipTechnique a rdfs:Class .

# Define properties
arco:hasTechnique a rdf:Property ;
                   rdfs:domain arco:ClothingItem ;
                   rdfs:range arco:CraftsmanshipTechnique .
arco:description a rdf:Property ;
                  rdfs:domain arco:CraftsmanshipTechnique ;
                  rdfs:range xsd:string .

# Create instances and relationships
<http://example.org/coat1> a arco:ClothingItem ;
                            arco:hasTechnique <http://example.org/tailoring> .

<http://example.org/tailoring> a arco:CraftsmanshipTechnique ;
                               arco:description "Tailoring involves precise cutting and sewing of fabric..."^^xsd:string .
```

In this RDF representation:

- We use the ArCo ontology to define classes for "ClothingItem" and "CraftsmanshipTechnique".
- We define properties "hasTechnique" and "description" to represent the relationship between a clothing item and its craftsmanship technique, and the description of the technique, respectively.
- We create instances of a coat (as a clothing item) and a specific craftsmanship technique (Tailoring).
- We establish a relationship between the coat and the Tailoring technique, and provide a description for the technique.

This RDF representation adheres to the ArCo ontology standards, making it compatible with other cultural heritage data represented using ArCo. You can replace `<http://example.org/>` with your preferred namespace URI.

- **LLAMA**

The ArCo clothing ontology is a great choice for describing the Cappotto, maschile. Here's the rewritten RDF code using the ArCo ontology:
```
@prefix arco: <http://www.w3.org/ns/arco/ontology#>.
@prefix dc: <http://purl.org/dc/terms/>.
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>.
<Cappotto, maschile>
a arco:Garment;
arco:hasType arco:Overcoat;
arco:hasDesigner <Novità Confezioni Italiane Eleganza>;
arco:hasOwner <Damiano Chiesa>;
arco:uses arco:CuttingAndPatternMaking;
arco:uses arco:SewingAndEmbroidery;
arco:uses arco:Tailoring;
arco:uses arco:FurriersSkills;
arco:uses arco:ButtonholeAndButtonAttachment;
arco:uses arco:FinishingTechniques;
arco:uses arco:QualityControl.
```
In this code, I've used the ArCo ontology to describe the Cappotto, maschile as a garment, specifying its type as an overcoat. I've also used ArCo properties to describe the garment's designer, owner, and the various craftsmanship techniques used in its creation.
Note that I've used the `a` keyword to indicate that the Cappotto, maschile is an instance of the `arco:Garment` class. I've also used ArCo properties such as `arco:hasType`, `arco:hasDesigner`, and `arco:hasOwner` to describe the garment's characteristics.

- **GEMINI**

Certainly! Here's the description transformed into RDF format using the ArCo clothing ontology with the two-part approach:

Part 1: Description of the Coat

```rdf
<rdf:Description rdf:about="http://example.org/cappotto_maschile">
  <dc:title>Cappotto, maschile – Novità Confezioni Italiane Eleganza (XX secolo)</dc:title>
  <arco:type rdf:resource="http://vocab.getty.edu/aat/300223001"/>  
  <arco:gender rdf:resource="http://vocab.getty.edu/aat/300100100"/>
  <f:owner rdf:resource="http://example.org/damiano_chiesa"/>  
  <f:productionPeriod rdf:datatype="http://www.w3.org/2001/XMLSchema#date">1901/01/01^^xsd:date</f:productionPeriod>
  <a-cd:subject rdf:resource="http://example.org/mens_tailoring_20th_century"/>
</rdf:Description>
```

Explanation (Part 1):

Same structure and explanation as before.

Part 2: Reference Description of Tailoring Techniques

```rdf
<rdf:Description rdf:about="http://example.org/mens_tailoring_20th_century">
  <dc:title>Men's Tailoring Techniques (20th Century)</dc:title>
  <arco:technique rdf:resource="http://vocab.getty.edu/aat/300132002"/> <arco:technique rdf:resource="http://vocab.getty.edu/aat/300132004"/>  
  <arco:technique rdf:resource="http://vocab.getty.edu/aat/300132011"/>  (Add more techniques as needed)
</rdf:Description>
```

Explanation (Part 2):

We kept the separate resource and title for the reference description.
We use the `arco:technique` property with specific URIs from the ArCo ontology to describe potential techniques:
    [http://vocab.getty.edu/aat/300132002](http://vocab.getty.edu/aat/300132002) - Tailoring (tailoring process)
    [http://vocab.getty.edu/aat/300132004](http://vocab.getty.edu/aat/300132004) - Hand-sewing (sewing by hand)
    [http://vocab.getty.edu/aat/300132011](http://vocab.getty.edu/aat/300132011) - Pad stitching (sewing to create padding)
You can further enrich this description by adding more techniques relevant to 20th-century men's coat tailoring (e.g., canvas construction, welt pockets).

This approach leverages the ArCo ontology for the coat itself and for describing potential tailoring techniques used during the creation of the garment. 

 **Question 1: Craftsmanship Techniques: When asked about the craftsmanship techniques used in a specific item of clothing:**

 - ChatGPT might provide a more detailed and context-rich description due to its extensive training.
 - LLAMA might offer a concise response, focusing on the key points without much elaboration.
 - Gemini might vary, potentially showing strengths in certain niche topics depending on its training data

 **Question 2: Main Topics Extraction: In zero-shot prompting:**

 - ChatGPT's answer might be comprehensive, leveraging its broad training data to cover multiple aspects.       
 - LLAMA might provide a more direct and focused list.      
 - Gemini could differ in its ability to extract and prioritize topics based on its unique training and tuning.

 **Question 3: RDF Format Transformation: Chain-of-thought prompting:**

 - ChatGPT is likely to break down the steps in a detailed manner.
 - LLAMA might provide a step-by-step guide but in a more concise format.
 - Gemini might show variability in depth and clarity based on how well it was trained on similar tasks.

 **Question 4: Using ArCo Ontology: Generated-knowledge prompting:**

 - ChatGPT might integrate previous responses effectively, providing a coherent and contextually aware answer.
 - LLAMA might excel in consistency and relevance.
 - Gemini might have varying results depending on its data integration capabilities.


>
## [SPARQL QUERIES](./another-page2.html)


[back](./)
