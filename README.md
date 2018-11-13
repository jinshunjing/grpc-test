# grpctest
Test gRPC

# Generate the java code
1. cd grpc
2. Uncomment the extension os-maven-plugin and protobuf-maven-plugin in pom.xml
2. mvn verify
3. cp -r target/generated-sources/protobuf/grpc-java/org src/main/java
4. cp -r target/generated-sources/protobuf/java/org src/main/java

# Run Server
mvn clean
mvn package
java -jar target/grpc-1.0-SNAPSHOT.jar

# Run Client
Run org.jim.grpc.hello.HelloClient in IDEA
