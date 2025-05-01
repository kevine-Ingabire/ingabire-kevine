FROM eclipse-temurin:23-jdk

WORKDIR /app

COPY OOP_Assignment/src ./src

RUN find src -name "*.java" > sources.txt \
 && cat sources.txt \
 && javac @sources.txt -d out \
 && echo "Compilation complete" \
 && ls -R out

CMD ["java", "-cp", "out", "task.Question1.MissionManagementMain"]