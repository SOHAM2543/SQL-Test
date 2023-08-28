SELECT
    point1.x AS x1,
    point1.y AS y1,
    point2.x AS x2,
    point2.y AS y2,
    SQRT(POW(point2.x - point1.x, 2) + POW(point2.y - point1.y, 2)) AS shortest_distance
FROM
    points AS point1
CROSS JOIN
    points AS point2
WHERE
    point1.point_id <> point2.point_id
ORDER BY
    shortest_distance
LIMIT 1;
