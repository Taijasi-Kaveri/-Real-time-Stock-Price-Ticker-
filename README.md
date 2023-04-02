# -Real-time-Stock-Price-Ticker-
This project is a real-time stock price ticker implemented using Core Java and Apache Kafka. The system reads stock price data from a data provider and publishes the data to a Kafka topic. The data can be consumed by a Java application that displays the prices in real-time using a user interface library such as Swing or JavaFX.

## Setup
To run the project, you'll need to follow these steps:

* Download and install Apache Kafka from the official website.
* Start the ZooKeeper server using the command bin/zookeeper-server-start.sh config/zookeeper.properties.
* Start the Kafka broker using the command bin/kafka-server-start.sh config/server.properties.
* Create a Kafka topic named "stock-prices" using the command bin/kafka-topics.sh --create --topic stock-prices --bootstrap-server localhost:9092.
* Choose a data provider that provides real-time stock price data via a REST API.
* Write a Java application that connects to the data provider's REST API and retrieves the stock price data.
* Parse the response and extract the relevant data such as the symbol, price, and timestamp.
* Use the Kafka Java client API to publish the data to the "stock-prices" topic.
* Write a Java application that listens to the "stock-prices" topic using the Kafka Java client API.
* Parse the message payload and extract the relevant data such as the symbol, price, and timestamp.
* Update the user interface with the latest stock price data.
* Use a user interface library such as Swing or JavaFX to create a ticker display that scrolls through the latest stock prices in real-time.
* Add error handling and logging to the application.

## Dependencies
* Java Runtime Environment (JRE) 8 or later
* ZooKeeper

## Usage
To use the project, you'll need to:

* Start the data provider application and make sure it successfully publishes stock price data to the "stock-prices" topic.
* Start the ticker application and make sure it successfully consumes and displays the stock price data in real-time.
* Test error handling and make sure any errors are logged appropriately.

## Credits
This project was created by me.

## License
This project is licensed under the [License Name] License. See the LICENSE file for more information.



