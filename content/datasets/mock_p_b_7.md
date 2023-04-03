---
hidden: no
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.123/tus-78gh4"
  name: "Mock data 19"
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
  copyrightYear: 2019
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
  dateCreated: "2019-11-19"
  datePublished: "2019-11-19"
  dateModified: "2019-11-21"
  keywords: "Pathology, Whole slide imaging, Breast, Lymph nodes, Cancer, Sentinel nodes, Immunohistochemical staining, cytokeratin, CKAE1/AE3"
  version: "1.0.2"
  # v1.0.2 2020-07-05: Update size in bytes.
  description: |
    Whole slide imaging of 396 full cases of axillary lymph nodes in breast
    cancer cases. 
  license:
  - name: "Controlled access"
    id: "https://datahub.bp.mock.se/mock#controlled-access"
    "@type": "CreativeWork"
    abstract: |
      Free for use in legal and ethical medical diagnostics research.
  - name: "Bigpicture license"
    id: "https://d"
  citation:
    #- "@type": "CreativeWork"
    #  "@id": "https://doi.org/..."
    #  name: "Title of paper goes here"
other:
  shortName: "MD19"
  status: "Ongoing"
  annotation: |
    No in-image annotations available. Additional information at case level
    available on request.
  countries-shared:
  - "FI"
  - "NO"
  - "SE"
  organ:
  - name: "Breast"
    sctid: 38498374 # SNOMED-CT https://termbrowser.nhs.uk/?perspective=full&conceptId1=%s
  age-span: "-"
  bytes: 2363159897649  # 2.4 TB
  numberOfScans: 4462
  numberOfAnnotations: 0
  resolution: "20x"
  modality:
  - "SM"
  scanner:
  - Aperio ScanScope AT
  - Hamamatsu NanoZoomer XR
  - Hamamatsu NanoZoomer S360
  - Hamamatsu NanoZoomer S60
  stain: "Hematoxylin and eosin. In sentinel node cases also immunohistochemical stain  for cytokeratin AE1/AE3."
  image: "img/m_p_b/wsi-thumbnail.jpeg"
  exampleImage:
  - title: "Overview of whole slide imaging with hematoxylin and eosin staining."
    url: "/assets/images/mock_datasets/bp/m_p_b/he-overview.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/he-overview-thumbnail.jpeg"
  - title: "Overview of whole slide imaging with cytokeratin immunostaining."
    url: "/assets/images/mock_datasets/bp/m_p_b/ckae-overview.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/ckae-overview-thumbnail.jpeg"
  - title: "Detail view of metastasis with hematoxylin and eosin staining."
    url: "/assets/images/mock_datasets/bp/m_p_b/he-metastasis.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/he-metastasis-thumbnail.jpeg"
  - title: "Detail view of metastasis with cytokeratin immunostaining."
    url: "/assets/images/mock_datasets/bp/m_p_b/ckae-metastasis.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_b/ckae-metastasis-thumbnail.jpeg"
access: Indirect
---
## File formats
### Pixel position scaling
Coordinates given are relative to the image *width*. To get the correct pixel
position, X coordinates (and Y coordinates!) should therefore be multiplied with
the image *width*.

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
