# Faircorp-REST-API
## API Documentation
### Windows Endpoints
#### Get Windows List:
- Request Type: GET
- Endpoint: /api/windows

#### Get Window With A Specific ID:
- Request Type: GET
- Endpoint: /api/windows/{windowId}
- {windowId}: A Long Integer

#### Get List Of Windows That Belongs To The Same Room:
- Request Type: GET
- Endpoint: /api/windows/rooms/{roomId}
- {roomId}: A Long Integer
#### Create A New Window:
- Request Type: POST
- Endpoint: /api/windows
- Body:
    ```json
    {
      "id": 0,
      "name": "string",
      "roomId": 0,
      "roomName": "string",
      "windowStatus": "CLOSED"
    }
    ```

#### Delete A Window:
- Request Type: DELETE
- Endpoint: /api/windows/{windowId}
- {windowId}: A Long Integer

#### Update A Window Status( OPEN <-> CLOSED):
- Request Type: PUT
- Endpoint: /api/windows/{windowId}/switch
- {windowId}: A Long Integer

### Heaters Endpoints:
#### Get Heaters List:
- Request Type: GET
- Endpoint: /api/heaters

#### Get Heater With A Specific ID:
- Request Type: GET
- Endpoint: /api/heaters/{heaterId}
-{heaterId}: A Long Integer

#### Create A New Heater:
- Request Type: POST
- Endpoint: /api/heaters
- Body:
    ```json
    {
      "heaterStatus": "OFF",
      "id": 0,
      "name": "string",
      "power": 0,
      "roomId": 0,
      "roomName": "string"
    }
    ```
#### Delete A Heater:
- Request Type: DELETE
- Endpoint: /api/heaters/{heaterId}
- {heaterId}: A Long Integer

#### Update A Heater Status(ON <-> OFF):
- Request Type: PUT
- Endpoint: /api/heaters/{heaterId}/switch
- {heaterId}: A Long Integer

### Rooms Endpoints:

#### Get Rooms List:
- Request Type: GET
- Endpoint: /api/rooms

#### Get Room With A Specific ID:
- Request Type: GET
- Endpoint: /api/rooms/{roomId}
- {roomId}: A Long Integer

#### 