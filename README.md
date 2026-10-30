
# Virtual Rocket Engine Test Stand Simulator

## Project Overview

The Virtual Rocket Engine Test Stand Simulator is a Python-based
engineering software project designed to simulate an engine test
environment, collect virtual sensor telemetry, monitor system
conditions, identify anomalies, and store historical test data.

The project demonstrates how software engineering, data analysis,
database management, and interactive visualization can be combined
into an integrated monitoring application.

All sensor readings and test sequences are simulated.
The application does not control physical hardware.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- SQLite
- IPyWidgets
- ReportLab
- Google Colab

## System Architecture

The application is organized into several interconnected modules.

1. Simulation Engine
   Generates virtual sensor readings and manages test sequences.

2. Telemetry Acquisition
   Collects and organizes simulated sensor measurements.

3. Monitoring Dashboard
   Displays sensor readings, system status, and performance graphs.

4. Safety Monitoring
   Evaluates configured sensor thresholds and generates warnings.

5. Sensor Diagnostics
   Simulates sensor faults, including missing data, stuck readings,
   and abnormal measurements.

6. Anomaly Detection
   Uses statistical analysis and median absolute deviation to
   identify unusual telemetry readings.

7. Database Management
   Uses SQLite to store telemetry records and event history.
   Each saved snapshot receives a unique run identifier.

8. Performance Analysis
   Compares historical test runs and calculates sensor statistics.

9. Automated Reporting
   Generates downloadable PDF reports containing test information,
   sensor statistics, safety results, and event history.

## Virtual Sensor Measurements

The simulator monitors six virtual sensors:

- Chamber Pressure
- Engine Temperature
- Fuel Flow
- Oxidizer Flow
- Vibration
- Tank Pressure

## Major Features

- Virtual test sequence execution
- Interactive operator controls
- Live telemetry visualization
- Sensor fault injection
- Automated safety evaluation
- Statistical anomaly detection
- SQLite database integration
- Historical test-run comparison
- CSV data export
- Automated PDF report generation
- Unified engineering operations dashboard

## Data Management

Telemetry records are organized using Pandas and stored in
a SQLite database.

The database contains two primary tables:

### Telemetry

Stores:
- Run identifier
- Simulation time
- Timestamp
- Sensor measurements

### Events

Stores:
- Run identifier
- Timestamp
- Event description

## Engineering Concepts Demonstrated

- Object-oriented programming
- Software modularity
- Data acquisition and processing
- Statistical analysis
- Database design and SQL queries
- Fault detection
- System monitoring
- Data visualization
- Automated reporting
- Software integration

## Running the Project

The project was developed in Google Colab.

To run it:

1. Open the notebook in Google Colab.
2. Execute the notebook cells in order.
3. Initialize the simulation environment.
4. Run a virtual test sequence.
5. Explore the monitoring dashboards.
6. Run diagnostics and anomaly detection.
7. Save telemetry to SQLite.
8. Compare test runs.
9. Generate a PDF test report.

## Project Limitations

This is a software-only simulation.

Sensor values, test phases, safety thresholds, and diagnostic
conditions are illustrative. They are not validated engineering
limits and must not be used for real propulsion operations.

The SQLite database is stored in the notebook environment.
Google Colab temporary storage may be cleared when its runtime
is disconnected.

## Future Enhancements

Potential improvements include:

- Real-time MQTT telemetry ingestion
- REST API integration
- Web-based monitoring interface
- Additional sensor simulation models
- More advanced statistical diagnostics
- Automated test-run scheduling
- Cloud database integration
- Unit and integration testing

## Author

Cameron D. Frost

Computer Science

Mississippi State University
