## Timezones

This is a list of all the timezone names along with their offset in seconds from UTC and also offset during daylight
savings time from UTC.

The format of the CSV is simply

```
timezone,offset,offset_dst
```


### Example MySQL database structure:

```
CREATE TABLE `timezones` (
  `timezoneid` SMALLINT(6) UNSIGNED NOT NULL AUTO_INCREMENT,
  `name`       VARCHAR(100)         NOT NULL DEFAULT '',
  `offset`     INT(10)              NOT NULL DEFAULT '0',
  `offset_dst` INT(10)              NOT NULL DEFAULT '0',
  PRIMARY KEY (`timezoneid`),
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```
