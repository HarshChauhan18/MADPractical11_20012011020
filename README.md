# MADPractical11_20012011020
Study: SQlite Database, RecyclerView, Broadcast Receiver, Service, Notification, Custom Alert Dialog Box, Time Picker Dialog, AlarmManager

AIM: Create Note Android Application that can add Note, edit Note, delete Note, and set reminder date & time of note. By using Broadcast Receiver, AlarmManager set reminder of note. By using SQLite, store all notes data.

Create two Activities like MainActivity, NoteViewActivity according to below UI design.

Use RecyclerView Code from Practical-9 to display Note Data.

Use Broadcast Receiver, Time Picker Dialog, service & AlarmManager code from Practical-7

Create Note class with member variables like id, title, subTitle, Description, modifiedTime, reminderTime:Long, isReminderEnable:Boolean & create membor methods like getCurrentDateTime(), getMillis(), setReminder(), isValid(), getReminderText(), saveNote(), getHour(), getMinute(), calculateReminder()

Create DatabaseHelper Class for SQlite with member methods like insertNote(), getNote(id), getAllNotes(), getNotesCount(), updateNote(), deleteNote().

Use Databinding in gradle file to easy way integrate xml into kotlin file

Use Material 3 design for UI

create class NotesData with companion object and it will store column name of table and create table query.

Create NoteViewActivity. It will show while reminder notification is turned up and user click on notification. It will also show when click on Note in recyclerView. After clicking on notification NoteViewActivity should be open with full description of that note.

Note should be deleted by clicking on icon of Delete. Note should not be added if any one field of note is empty.

Some notes have reminder time so add reminder time in alarmManager with note id & it should be receive in broadcast receiver & in broadcast receiver notification should be generated with title & description of note.

If More than one notes have reminder time then notification should be displayed for each note separately.

Create Common Custom Dialog Box for add, edit note.

Create RecyclerView & its adapter to display all notes.

Output :

![image](https://user-images.githubusercontent.com/107744227/202469249-fbac64b1-e8ba-404d-b4f4-9ca2eecd837a.png)

![image](https://user-images.githubusercontent.com/107744227/202469372-308b1a7a-e0ab-4e10-b0fc-b09eedde1038.png)

![image](https://user-images.githubusercontent.com/107744227/202469419-09506ed5-acf5-4ced-8dbd-a15eafd66608.png)

![image](https://user-images.githubusercontent.com/107744227/202469463-f66ac298-b4b1-4254-9d8c-902c40dc24e7.png)



