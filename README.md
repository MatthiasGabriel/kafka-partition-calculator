# Kafka Partition Calculator

A simple web tool to calculate the target partition for Kafka message keys using the murmur2 algorithm.

## Live Demo
**https://thiko.github.io/kafka-partition-calculator**

## Usage
1. Enter your message key (e.g., "user123", "order-456")
2. Enter the number of partitions
3. View the calculated target partition

## Running Locally
Open `index.html` in any web browser. No build process required.

## Algorithm
Uses the same logic as Apache Kafka:
```
partition = abs(murmur2(messageKey)) % partitionCount
```

## Features
- Real-time calculation
- Murmur2 hash (same as Kafka)
- Responsive design
- No dependencies

## License
MIT