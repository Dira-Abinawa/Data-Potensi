**README.md**

# Dira Abinawa - Data Potensi

This is a FastAPI application for managing data related to potential school members in the Dira Abinawa project.

## Requirements

Make sure you have the following installed before running the application:

- Python 3.x
- FastAPI
- Pydantic
- pymongo
- MongoDB

## Installation

1. Clone this repository to your local machine.
2. Install the required packages using pip:

   ```bash
   pip install fastapi
   pip install uvicorn
   pip install pymongo
   ```

## Configuration

1. Ensure you have a running MongoDB instance with the appropriate credentials.
2. Update the `connection` variable in the `app.py` file with the correct MongoDB connection string and collection name.

## Running the Application

1. Navigate to the root directory of the project.
2. Start the FastAPI application using the `uvicorn` command:

   ```bash
   uvicorn app:app --reload
   ```

3. The application should now be running locally and accessible at `http://localhost:8000`.

## API Endpoints

### GET /data_potensi

Retrieves a list of all potential school members.

### POST /data_potensi

Creates a new potential school member.

### PUT /data_potensi/{id}

Updates an existing potential school member based on the provided ID.

### DELETE /data_potensi/{id}

Deletes a potential school member based on the provided ID.

## DataPotensi Model

The `DataPotensi` model is used to represent a potential school member. It includes the following attributes:

- school_name (string)
- male_builder (integer)
- female_builder (integer)
- male_member (integer)
- female_member (integer)
- bantara_member (integer)
- laksana_member (integer)
- garuda_member (integer)

Please note that some attributes are optional and may have a value of `None`.

## Acknowledgments

- [FastAPI Documentation](https://fastapi.tiangolo.com/)
- [Pydantic Documentation](https://pydantic-docs.helpmanual.io/)
- [MongoDB Documentation](https://docs.mongodb.com/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.# Data-Potensi
