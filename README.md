# connected_drive.js
ES6 module to access BMW Connected Drive API.

# Example usage
```javascript
const connected_drive = require("connected_drive.js");

// Authenticate with BMW API.
let account = await connected_drive.auth(
  username,
  password
);

// Find a vehicle with known vehicle identification.
let vehicle = await account.findVehicle(vehicle_id);

// Flash it's headlights.
vehicle.flashLights();
```

# Acknowledgements
Inspired by https://github.com/bimmerconnected/bimmer_connected
