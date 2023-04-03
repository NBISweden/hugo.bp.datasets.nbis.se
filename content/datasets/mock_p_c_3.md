---
hidden: no
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.123/rc6ea5c0g"
  name: "Mock data 24"
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
  dateCreated: "2019-11-19"
  datePublished: "2019-11-19"
  dateModified: "2019-11-21"
  keywords: "Pathology, Colon, Cancer, Whole slide imaging, Annotated"
  version: "1.1.0"
  # v1.1.0 2020-11-27: Add citation.
  # v1.0.2 2020-07-05: Update size in bytes.
  description: |
    The dataset consists of 101 H&E-stained colon whole slide images (WSI)
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
  shortName: "MD24"
  status: "Completed"
  annotation: No in-image annotations available. Additional information at case level
    available on request.    
  countries-shared:
    - "CH"
    - "FI"
    - "NO"
    - "SE"
  organ:
  - name: "Colon"
    sctid: BBV3
  age-span: "22-90 years"
  bytes: 49227373916 # 49 GB
  numberOfScans: 101
  numberOfAnnotations: 756
  resolution: "20X and 40X single plane"
  modality:
  - "SM"
  scanner:
  - "Scanscope AT (Aperio, US)"
  - "NanoZoomer XR (Hamamatsu, Japan)" # FIXME: is this same as "Hamamatsu NanoZoomer-XR C12000 series 2013"?
  - "NanoZoomer XRL (Hamamatsu, Japan)" # FIXME: is this same as "Hamamatsu NanoZoomer 2.0 HT C9600 series 2013"
  stain: "H&E (hematoxylin and eosin)"
  phase:
  image: "img/m_p_c/primary-tumor-thumbnail.jpeg"
  exampleImage:
  - title: "Overview of whole slide imaging."
    url: "/assets/images/mock_datasets/bp/m_p_c/primary-tumor.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_c/primary-tumor-thumbnail.jpeg"
  - title: "Overview of annotations."
    url: "/assets/images/mock_datasets/bp/m_p_c/annotations.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_c/annotations-thumbnail.jpeg"
  - title: "Overview of carcinoma whole slide imaging."
    url: "/assets/images/mock_datasets/bp/m_p_c/carcinoma.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_c/carcinoma-thumbnail.jpeg"
  - title: "Overview of carcinoma annotations."
    url: "/assets/images/mock_datasets/bp/m_p_c/carcinoma-annotations.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_c/carcinoma-annotations-thumbnail.jpeg"
  - title: "To-scale view of pixel resolution in original whole slide imaging data."
    url: "/assets/images/mock_datasets/bp/m_p_c/to-scale.jpeg"
    thumbnail-url: "/assets/images/mock_datasets/bp/m_p_c/to-scale-thumbnail.jpeg"
access: Direct
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
