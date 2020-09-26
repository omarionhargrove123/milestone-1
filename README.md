# milestone-1
# Create a repository in your organization ~/Projects/my-project$ gh repo create my-cool-project ✓ Created repository user/my-cool-project on GitHub ✓ Added remote https://github.com/user/my-cool-project.git ~/Projects/my-project$
>sqlite3
SQLite version 3.29.0 2019-07-10 17:32:03
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite>
>sqlite3 c:\sqlite\db\chinook.db
SQLite version 3.13.0 2016-05-18 10:57:30
Enter ".help" for usage hints.
sqlite>
sqlite> .open c:\sqlite\db\chinook.db
>sqlite3 c:\sqlite\db\sales.db
SQLite version 3.29.0 2019-07-10 17:32:03
Enter ".help" for usage hints.
sqlite>
>sqlite3 c:\sqlite\db\sales.db
SQLite version 3.29.0 2019-07-10 17:32:03
Enter ".help" for usage hints.
sqlite>
>sqlite3 c:\sqlite\db\sales.db
SQLite version 3.29.0 2019-07-10 17:32:03
Enter ".help" for usage hints.
sqlite>
.help
sqlite> .database
seq  name             file
---  ---------------  --------------------------
0    main             c:\sqlite\db\sales.db
sqlite>
sqlite> ATTACH DATABASE "c:\sqlite\db\chinook.db" AS chinook;
>sqlite3 c:\sqlite\db\chinook.db
SQLite version 3.29.0 2019-07-10 17:32:03
Enter ".help" for usage hints.
sqlite> .tables
albums          employees       invoices        playlists
artists         genres          media_types     tracks
customers       invoice_items   playlist_track
sqlite>
sqlite> .indexes
IFK_AlbumArtistId
IFK_CustomerSupportRepId
IFK_EmployeeReportsTo
IFK_InvoiceCustomerId
IFK_InvoiceLineInvoiceId
IFK_InvoiceLineTrackId
IFK_PlaylistTrackTrackId
IFK_TrackAlbumId
IFK_TrackGenreId
IFK_TrackMediaTypeId
