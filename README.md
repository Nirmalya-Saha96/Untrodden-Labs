# Untrodden-Labs
db.weather.aggregate(
   [
     {
       $group:
         {
           _id: "$weather.sensorId",
           tempAve: { $avg: "$temp" }
         }
     }
   ]
)
