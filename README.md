# easy-xml

**_easy-xml_** is a small library aimed for easy creation and parsing of xml's.

## Simple Usage

### Parsing

#### Simple Xml

```javascript
const xml = requre("easy-xml");

const xmlString = `
<movies>
  <movie>
    <title>Awesome Movie 1</title>
    <producer>Disney's Pixar</producer>
    <director>John Doe</director>
  </movie>
  <movie>
    <title>Awesome Movie 2</title>
    <producer>Twenty Century Fox</producer>
    <director>Sam Smith</director>
  </movie>
</movies>
`;

const parsedXml = xml.parse(xmlString);
/*
This will produce:

{
  movies: {
    movie: [
      {
        title: "Awesome Movie 1",
        producer: "Disney's Pixar",
        director: "John Doe"
      },
      {
        title: "Awesome Movie 2",
        producer: "Twenty Century Fox",
        director: "Sam Smith"
      }
    ]
  }
}
*/
```
