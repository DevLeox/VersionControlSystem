# Version Control System 📜

A lightweight **Java-based version control system** to manage and track versions of content with corresponding change logs. This tool can assist developers and teams in maintaining a structured and accessible record of project versions.

---

## Features ✨

- **Add Versions**: Save new versions along with their change logs.
- **Retrieve Content**: Access the content of a specific version.
- **Track Changes**: View the change log of any version.
- **Compare Versions**: Check if two versions are identical or different.
- **List All Versions**: See a comprehensive list of all stored versions with metadata.

---

## Usage 💻

### Add a Version:
```java
VersionControlSystem vcs = new VersionControlSystem();
int versionNumber = vcs.addVersion("Initial content", "Created the base version.");
System.out.println("New version added: " + versionNumber);
```

### Retrieve Content:
```java
String content = vcs.getVersionContent(versionNumber);
System.out.println("Version Content: " + content);
```

### Retrieve Change Log:
```java
String changeLog = vcs.getVersionChangeLog(versionNumber);
System.out.println("Change Log: " + changeLog);
```

### List All Versions:
```java
List<String> allVersions = vcs.listAllVersions();
allVersions.forEach(System.out::println);
```

### Compare Two Versions:
```java
String comparison = vcs.compareVersions(1, 2);
System.out.println("Comparison Result: " + comparison);
```

---

## Code Overview 🛠️

### `VersionControlSystem.java`

The **`VersionControlSystem`** class includes:
- **Attributes**:
  - `versions`: A `Map` to store version content.
  - `changeLogs`: A `Map` to store change logs of each version.
  - `versionCount`: An integer to track the number of versions.
- **Core Methods**:
  - `addVersion(String content, String changeLog)`: Adds a new version.
  - `getVersionContent(int versionNumber)`: Retrieves content of a specific version.
  - `getVersionChangeLog(int versionNumber)`: Retrieves the change log of a version.
  - `listAllVersions()`: Returns all versions in a list format.
  - `compareVersions(int version1, int version2)`: Compares the content of two versions.

---

## How to Run 🚀

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YourUsername/VersionControlSystem.git
   cd VersionControlSystem
   ```

2. **Compile and Run**:
   ```bash
   javac com/LeoxDev/VersionControlSystem/VersionControlSystem.java
   java com.LeoxDev.VersionControlSystem.VersionControlSystem
   ```

---

## Contributing 🤝

Contributions are welcome! Open an issue or submit a pull request to help improve this version control system.

---

## License 📜

This project is licensed under the MIT License. Feel free to use, modify, and distribute as per the license terms.
