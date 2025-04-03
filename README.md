# Multi-Format Data Converter 📜

A lightweight **Java-based tool** designed to convert data between JSON, XML, and HTML formats. This project helps developers handle multi-format data with ease, making it ideal for projects requiring simple and efficient data transformation.

---

## Features ✨

- **JSON to XML**: Convert JSON strings to XML format.
- **JSON to HTML**: Transform JSON strings into readable HTML.
- **XML to JSON**: Process XML data and turn it into JSON format.
- **XML to HTML**: Convert XML strings into HTML.
- **HTML to JSON**: Parse HTML content and turn it into JSON.
- **HTML to XML**: Convert HTML strings back into XML.

---

## Usage 💻

### Convert JSON to XML:
```java
String xmlOutput = ConvertJson.jsonToXml("{\"name\":\"John\", \"age\":\"30\"}");
System.out.println("Converted XML: \n" + xmlOutput);
```

### Convert XML to JSON:
```java
String jsonOutput = ConvertXml.xmlToJson("<name>John</name><age>30</age>");
System.out.println("Converted JSON: \n" + jsonOutput);
```

### Convert HTML to XML:
```java
String xmlOutput = ConvertHtml.htmlToXml("<p>name: John</p><p>age: 30</p>");
System.out.println("Converted XML: \n" + xmlOutput);
```

---

## Code Overview 🛠️

This repository includes three main classes:
- **ConvertJson**: Handles conversions between JSON and XML/HTML formats.
- **ConvertXml**: Transforms XML into JSON/HTML formats.
- **ConvertHtml**: Converts HTML to JSON/XML formats.

Each class has two methods for specific transformations and operates entirely on input strings.

---

## How to Run 🚀

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/DevLeox/Converter.git
   cd Converter
   ```

2. **Compile and Run**:
   ```bash
   javac ConvertJson.java ConvertXml.java ConvertHtml.java
   java ConvertJson
   ```

---

## Contributing 🤝

Contributions are welcome! Feel free to open an issue or pull request for suggestions or enhancements.

---

## License 📜

This project is licensed under the MIT License. Modify and use it as needed.
