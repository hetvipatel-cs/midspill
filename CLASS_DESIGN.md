Class: ReadingList

Attributes: 
- ArrayList<Book>: ArrayList

Relationships:
- Has Book Objects

Responsibilities:
- Manage Book Objects and sort them by the appropriate attribute

Class: Book

Attributes:
- title: String
- author: String
- pages: int
- genre: String
- ISBN: String
- rating: double
- readingStatus: String

Relationships:
- Organized in the ReadingList Class

Responsibilities:
- Store information about books
- Allow users to change any information necessary
- Organize books in an ArrayList as they are added

Class: Journal

Attributes:
- title: String
- type: String
- content: String

Relationships:
- N/A

Responsibilities:
- ability to update title and type
- Update and store content

Class: Story

Attributes:
- title: String
- shortDescription: String
- ArrayList<StoryCharacter>: ArrayList
- ArrayList<Chapter>: ArrayList

Relationships:
- Has Chapters and Characters

Responsibilities:
- ability to add/edit/delete characters
- ability to add/edit/delete chapters
- ability to modify title and description

Class: Chapter

Attributes:
- title: String
- type: String
- content: String

Relationships:
- Is used in the Story class

Responsibilities:
- ability to edit attributes
- Stores and updates content

Class: StoryCharacter

Attributes:
- name: String
- characterType: String
- description: String
- isMainCharacter: boolean

Relationships:
- Is used in the Story class

Responsibilities:
- ability to edit attributes

Class: Main

Attributes:
- N/A

Relationships:
-Utilizes all prior mentioned classes directly and/or indirectly

Responsibilities:
- Asks user for input regarding Stories, Books, Journals, Chapters, and StoryCharacters
- Updates information in the appropriate class(s)
- Handles bad input
