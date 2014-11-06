# RailsStats

See stuff about a Rails app.

```bash
$ bundle exec rake:stats[/users/me/path/to/app/]

Directory: /users/me/path/to/app/

+----------------------+-------+-------+---------+---------+-----+-------+
| Name                 | Lines |   LOC | Classes | Methods | M/C | LOC/M |
+----------------------+-------+-------+---------+---------+-----+-------+
| Controllers          |  1848 |  1483 |      32 |     174 |   5 |     6 |
| Helpers              |  2257 |  1892 |      45 |     245 |   5 |     5 |
| Jobs                 |   399 |   295 |      11 |      33 |   3 |     6 |
| Models               |  4584 |  3509 |      61 |     526 |   8 |     4 |
| Observers            |    42 |    22 |       2 |       5 |   2 |     2 |
| Libraries            |  2987 |  2272 |      30 |     287 |   9 |     5 |
| Configuration        |  1233 |   669 |       4 |      17 |   4 |    37 |
| Spec Support         |  1416 |  1152 |       4 |      30 |   7 |    36 |
| Integration Tests    |    91 |    73 |       0 |       1 |   0 |    71 |
| Lib Tests            |   101 |    83 |       0 |       1 |   0 |    81 |
| Model Tests          |  3397 |  2522 |       0 |      18 |   0 |   138 |
| Cucumber Support     |   739 |   521 |       0 |       1 |   0 |   519 |
| Cucumber Features    |  2711 |  2487 |      29 |     145 |   5 |    15 |
+----------------------+-------+-------+---------+---------+-----+-------+
| Total                | 21805 | 16980 |     218 |    1483 |   6 |     9 |
+----------------------+-------+-------+---------+---------+-----+-------+
  Code LOC: 10142     Test LOC: 6838     Code to Test Ratio: 1:0.7

```

### Things it knows about

* Any concepts you've added within an `app` directory
* Configuration files
* Library files
* Gems that you've embedded in the project
* Engines and their code
* RSpec and Cucumber Tests

### TODO

* Option to print out by app directory (stats per engine)
* Add views (jbuilder, erb, haml) but don't count towards ratios
* Support JS for projects that have it in public (but not compiled)
* Add CSS but don't count towards ratios
* Output other metrics like number of tables and columns
* Test unit support
* Different output formatters
