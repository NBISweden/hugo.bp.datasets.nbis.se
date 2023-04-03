---
hidden: no
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.123/8u90uvx0z"
  name: "Mock data 9"
  about: "Pathology"
  url: "https:/.Mock"
  author:
  - name: "Person 1"
    #"@id": # FIXME: missing info
    "@type": "Person"
  - name: "Person 2"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  - name: "Person 3"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  - name: "Person 4"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  - name: "Person 4"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  - name: "Person 5"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  publisher:
    "@type": "Organization"
    name: "BP"
  copyrightYear: 2017
  copyrightHolder:
  - name: "University 1"
    url: "https://uni1.se/"
    "@type": "Organization"
  - name: "person 1"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  provider:
  - name: "Person 2"
    email: "person1@uni1.se"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  - name: "person 3"
    email: "person3@uni1.se"
    #"@id": "" # FIXME: missing info
    "@type": "Person"        
  - name: "Person 4"
    email: "Person4@uni1.se"
    "@id": "https://orcid.org/0"
    "@type": "Person"
  - name: "BP"
    email: "BP@mock.com"
    "@id": "https://datahub.bp.mock.se"
    "@type": "Organization"
  dateCreated: "2021-03-04"
  datePublished: "2021-03-23"
  dateModified: "2021-03-23"
  keywords: "Pathology, Annotated"
  version: "1.0"
  description: |
    This dataset contains 433
    radiographs from 149 patients with complete AFF.
  license:
  - name: "Controlled access"
    id: "https://datahub.bp.mock.se/mock/drco#controlled-access"
    "@type": "CreativeWork"
    abstract: |
      Free for use in legal and ethical medical diagnostics research.
  - name: "license"
    id: "https://datahub.bp.mock.se//mock#bp-by-license"
    "@type": "CreativeWork"
    abstract: "Free for use within BP with attribution."
 
other:
  shortName: "MD9"
  status: "Completed"
  countries-shared:
  - "SE"
  organ:
  - name: "Colon"
    sctid: 71341001 
  age-span: ""
  bytes: 3881258996
  numberOfScans: 981
  numberOfAnnotations: 981
  resolution:
  modality:
  - "SM"
  scanner:
  stain:
  phase:
  image: "img/m_r_f/to-scale (1).jpeg"
  exampleImage:
  - title: "Colon fracture radiograph with an AI generated heatmap indicating probable presence and location of an Atypical Colon Fracture."
    url: "/assets/images/mock_datasets/bp/m_r_f/to-scale (1).jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_r_f/to-scale-thumbnail (1).jpeg"
access: Indirect
---


## License






Copyright
{{ page.datacite.copyrightYear }}
{{ page.datacite.copyrightHolder | map: "name" |  join: ", " }}

Donec nibh elit, tincidunt eget vulputate ac, consequat in ipsum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Cras interdum enim at libero sodales finibus. Donec vitae lorem quam. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Phasellus eget orci vulputate quam porttitor dignissim. Maecenas commodo, nibh et iaculis blandit, leo arcu scelerisque tortor, id porttitor metus tortor commodo quam. Vivamus a dapibus ipsum, eu euismod elit.

{{ page.datacite.author | map: "name" | array_to_sentence_string }}
({{ page.datacite.datePublished | date: "%Y" }})
{{ page.datacite.name }}
[doi:{{ page.datacite['@id'] | remove: "https://doi.org/" }}]({{ page.datacite["@id"] }}).

 Integer tempus ullamcorper quam, eu consequat ante pulvinar ac. Nulla in ipsum mattis, congue orci vitae, rhoncus lacus. Aliquam nunc turpis, tincidunt in nibh eu, bibendum luctus diam. Praesent varius orci erat, nec sollicitudin tellus venenatis vel. Morbi quis ullamcorper arcu, quis ultricies odio.
