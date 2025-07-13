import java.io.*;

public class FileEditor {

	// Writes text to a file
	public static void writeToFile(String filename, String content) throws IOException {
		FileWriter writer = new FileWriter(filename);
		writer.write(content);
		writer.close();
		System.out.println("*Content written to file.");
	}

	// Reads and returns text from a file
	public static String readFromFile(String filename) throws IOException {
		BufferedReader reader = new BufferedReader(new FileReader(filename));
		StringBuilder content = new StringBuilder();
		String line;
		while ((line = reader.readLine()) != null) {
			content.append(line).append("\n");
		}
		reader.close();
		System.out.println("File content read successfully.");
		return content.toString();
	}

	// Modifies text in a file (by replacing a target word with a replacement)
	public static void modifyFile(String filename, String target, String replacement) throws IOException {
		String content = readFromFile(filename);
		content = content.replaceAll(target, replacement);
		writeToFile(filename, content);
		System.out.println("File content modified.");
	}

	public static void main(String[] args) {
		String filename = "sample.txt";
		String initialContent = "Java is powerful";

		try {
			writeToFile(filename, initialContent);
			String readContent = readFromFile(filename);
			System.out.println("Original Content:\n" + readContent);

			modifyFile(filename, "Java", "Python");
			String modifiedContent = readFromFile(filename);
			System.out.println("Modified Content:\n" + modifiedContent);
		} catch (IOException e) {
			System.out.println("Error: " + e.getMessage());
		}
	}

}
