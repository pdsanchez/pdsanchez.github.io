---
title: "Spark broadcast joins"
categories:
  - Utilidades
tags:
  - Utilidades
  - spark
---

```
peopleDF.join(
  broadcast(citiesDF),
  Seq("city")
)
  .explain()
```

Mejor:

```
peopleDF.join(
  broadcast(citiesDF),
  peopleDF("city") <=> citiesDF("city")
)
  .drop(citiesDF("city"))
  .explain()
```

- [https://mungingdata.com/apache-spark/broadcast-joins/](https://mungingdata.com/apache-spark/broadcast-joins/)