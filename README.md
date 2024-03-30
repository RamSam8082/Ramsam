import spark.*;

public class SimpleWebServer {
    public static void main(String[] args) {
        // Initialize Spark
        Spark.port(8080); // Set port number

        // Define routes
        Spark.get("/", (req, res) -> "Hello, World!"); // Define a route for the root URL

        // Start the server
        Spark.awaitInitialization(); // Wait for server to start
        System.out.println("Server started on port 8080");
    }
}
