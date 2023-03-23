---
hidden: no
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": 
  name: "Mock data from YAML 1"
  publisher:
    "@type": "Organization"
    name: "BP"
  copyrightYear: 
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
    "@id": "https://"
    "@type": "Organization"
  dateCreated: "2020-11-19"
  datePublished: "2020-11-19"
  dateModified: "2020-11-21"
  keywords: "Pathology, Whole slide imaging, Breast, Lymph nodes, Cancer, Sentinel nodes, Immunohistochemical staining, cytokeratin, CKAE1/AE3"
  version:
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
  - name: "Big picture license"
    id: "https://"
  citation:
    #- "@type": "CreativeWork"
    #  "@id": "https://doi.org/..."
    #  name: "Title of paper goes here"
other:
  age_at_extraction:
  - '45'
  - '90'
  anatomical_site:
  - Skin structure of cheek (body structure)
  - Skin structure of upper arm
  - Skin structure of lower leg (body structure)
  - Skin structure of back (body structure)
  - Skin structure of hand (body structure)
  - Skin appendage structure
  - Skin of knee
  animal_species:
  - Homo sapiens
  block_preparation: []
  bp_image_type:
  - Brightfield
  extraction_method:
  - Biopsy
  - Scraping
  - Excision
  image_resolution:
  - 0.00022984807042544878
  - 0.00046104195481788847
  indirect_access_only: 'False'
  specimen_type:
  - Histopathology
  staining_name:
  - "KIR\xD6D" 
  - KI67
  - P16
  - hematoxylin stain,water soluble eosin stain
  - "SOXR\xD6D"
  - CK18
  - MELAN
  - HSV1
  - HSV2
  - CKAE
  - SOX10
  - HMB,
  shortName: "MD1"
  status:
  annotation: |
    No in-image annotations available. Additional information at case level
    available on request.
  countries-shared:
  - "FI"
  - "NO"
  - "SE"
  organ:
  age-span: "-"
  bytes:
  numberOfScans:
  numberOfAnnotations:
  modality:
  scanner:
  - Aperio ScanScope AT
  - Hamamatsu NanoZoomer XR
  - Hamamatsu NanoZoomer S360
  - Hamamatsu NanoZoomer S60
  image: "/img/m_p_b/ckae-metastasis-thumbnail.jpeg"
  exampleImage:
  
  - title: "Overview of whole slide imaging with hematoxylin and eosin staining."
    url: "/img/m_p_b/he-overview.jpeg"
    thumbnail-url: "/img/m_p_b/he-overview-thumbnail.jpeg"
  - title: "Overview of whole slide imaging with cytokeratin immunostaining."
    url: "/img/m_p_b/ckae-overview.jpeg"
    thumbnail-url: "/img/m_p_b/ckae-overview-thumbnail.jpeg"
  - title: "Detail view of metastasis with hematoxylin and eosin staining."
    url: "/img/m_p_b/he-metastasis.jpeg"
    thumbnail-url: "/img/m_p_b/he-metastasis-thumbnail.jpeg"
  - title: "Detail view of metastasis with cytokeratin immunostaining."
    url: "/img/m_p_b/ckae-metastasis.jpeg"
    thumbnail-url: "/img/m_p_b/ckae-metastasis-thumbnail.jpeg"
access: Direct
---
## File formats
### Pixel position scaling
Coordinates given are relative to the image *width*. To get the correct pixel
position, X coordinates (and Y coordinates!) should therefore be multiplied with
the image *width*.


## License

Copyright
{{ .Params.datacite.copyrightYear }}
{{ page.datacite.copyrightHolder | map: "name" |  join: ", " }}

Donec nibh elit, tincidunt eget vulputate ac, consequat in ipsum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Cras interdum enim at libero sodales finibus. Donec vitae lorem quam. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Phasellus eget orci vulputate quam porttitor dignissim. Maecenas commodo, nibh et iaculis blandit, leo arcu scelerisque tortor, id porttitor metus tortor commodo quam. Vivamus a dapibus ipsum, eu euismod elit.

{{ page.datacite.author | map: "name" | array_to_sentence_string }}
({{ page.datacite.datePublished | date: "%Y" }})
{{ page.datacite.name }}
[doi:{{ page.datacite['@id'] | remove: "https://doi.org/" }}]({{ page.datacite["@id"] }}).

{{ range $author := .Params.datacite.author }}
  {{ $author.name }}{{ if not (eq $author $last) }},{{ end }}
{{ end }}
({{ .Params.datacite.datePublished | dateFormat "2006" }})
{{ .Params.datacite.name }}
[doi:{{ .Params.datacite["@id"] | replaceRE "^https://doi.org/" "" }}]({{ .Params.datacite["@id"] }})

 Integer tempus ullamcorper quam, eu consequat ante pulvinar ac. Nulla in ipsum mattis, congue orci vitae, rhoncus lacus. Aliquam nunc turpis, tincidunt in nibh eu, bibendum luctus diam. Praesent varius orci erat, nec sollicitudin tellus venenatis vel. Morbi quis ullamcorper arcu, quis ultricies odio.
