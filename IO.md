# Java IO

### BufferedReader

 <img src="image.png" alt="inline drawing" width="200px" style="float:right; margin-right:0px;" /> 

A BufferedReader is used to read data from a source in Java <br>



**Syntax:**

- `Path` variable to the .txt Document

```java
public void readFile(String path){
    try{
    BufferedReader reader = new BufferedReader(new FileReader(path))
    }
    catch(IOException e){
        e.printStackTrace();
    }
}
```

**Getting data from the Reader:**

```java
try{
String output = reader.readLine();
int age =Integer.parseInt( reader.readLine());
double weight = Double.parseDouble(reader.readLine());
}
catch(IOException e){
    e.printStackTrace();
}
```

---

### BufferedWriter

A BufferedWriter is used to "write" data to a specific destination (eg. a .txt file)

**Syntax:**

- `Path` variable to the .txt Document

```java
public void writeToFile(String path){
    try{
    BufferedWriter writer = new BufferedWriter(new FileWriter(path))
    }
    catch(IOException e){
        e.printStackTrace();
    }
}
```

**Writing Data with the Writer:**

```java
try{
writer.write(age);
writer.write(name);
writer.write(weight);
}
catch(IOException e){
    e.printStackTrace();
}
```
--- 

