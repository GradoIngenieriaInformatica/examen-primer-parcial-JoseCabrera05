# Pregunta 5

```javascript
use biblioteca

db.libros.aggregate([
  {
    $group: {
      _id: "$categoria",
      total: { $sum: 1 }
    }
  },
  {
    $sort: { total: -1 }
  }
])
```
