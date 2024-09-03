# Musical Performances OOP Project
## Overview
This Java project simulates musical performances while demonstrating key Object-Oriented Programming (OOP) concepts such as inheritance, encapsulation, abstraction, polymorphism, and interface implementation. The program models various aspects of a musical performance including main artists, backup singers, backup dancers, music tracks, and the distinction between live and studio performances.

## Features
Main Artist: The lead performer in each musical performance (e.g., Taylor Swift).
Performance Attributes: Includes performance name, year, venue, track list, backup singers, and backup dancers.
Track List: A variable number of music tracks with a name and duration (e.g., "Lavender Haze", 3.22 minutes).
Backup Singers and Dancers: The performance is supported by backup singers (who sing) and dancers (who dance).
Two Types of Performances:
Live Performance: Allows artist interaction with the audience and is recorded differently from studio performances.
Studio Performance: Includes audio processing functionality.
Recording: Both live and studio performances can be recorded, but they use different recording methods.
Interface IBackup: Used for defining backup behavior for singers and dancers.
## Classes
Performance: The base class that defines the structure of a musical performance, including attributes like the main artist, year, venue, and track list.
LivePerformance: Inherits from Performance, allows audience interaction, and implements the Record interface for recording live performances.
StudioPerformance: Inherits from Performance, implements the Record interface, and includes audio processing functionality for studio performances.
Artist: The base class representing any artist involved in the performance, whether they are the main artist, a backup singer, or a backup dancer.
Singer: Inherits from Artist and adds singing functionality.
MainArtist: Inherits from Singer and represents the main artist of the performance.
BackUpSinger: Inherits from Singer and implements the IBackup interface to assist the main artist by singing.
BackUpDancer: Inherits from Artist and implements the IBackup interface to assist the main artist by dancing.
Track: Represents a music track with a name and duration (modeled as a HashMap in the program).
Interfaces:
IBackup: An interface for backup performers, defining the backUp method.
Record: An interface defining the record method for recording performances.
