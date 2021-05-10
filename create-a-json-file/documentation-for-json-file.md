---
description: Documenting an JSON file
---

# Documentation for JSON file

Let us create documentation for JSON file with structured data that will register the library patron’s activity in the system.

**library** is the _main object_ that will contain _librarian_ and _library patron_ as two objects. The actions that will be carried out by the librarian and the patron will form the _item objects._

**Top Level:** _library menu object_

| Component | Description | Type |
| :--- | :--- | :--- |
| library |  Actions performed by the librarian and library patron | library component |

**library component**: Represents the _column objects_, librarian, and library patron.

| Component | Description | Type |
| :--- | :--- | :--- |
| librarian | Collects data daily | Library component |
| library patron | Borrows books from library and returns within the estimated date | Library component |

**library patron:** Represents the _item objects_ of the patron, which are the actions that can be performed.

| Component |  | Description | Type | Notes |
| :--- | :--- | :--- | :--- | :--- |
| Check out |  | List of items under the column | An array of menu items |  |
|  | Book title | The name of the book borrowed | string |  |
|  | Check-out date | The date when the book was borrowed | string | Format: dd-mm-yyyy |
| Check in |  | List of items under the column | An array of menu items |  |
|  | Book title | The name of the book returned | string |  |
|  | Check-in date | The date when thebook must be returned | string | Format: dd-mm-yyyy |
| Pay fine | Penalty for delay or misplacing book | number |  |  |

**librarian:** Represents the _item objects,_ which are the actions that can be carried out by the librarian.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Component</th>
      <th style="text-align:left"></th>
      <th style="text-align:left">Description</th>
      <th style="text-align:left">Type</th>
      <th style="text-align:left">Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Check out</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">List of items under the column</td>
      <td style="text-align:left">An array of menu items</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Book title</td>
      <td style="text-align:left">The name of the book borrowed</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Check-out date</td>
      <td style="text-align:left">Books borrowed</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">Format: dd-mm-yyyy</td>
    </tr>
    <tr>
      <td style="text-align:left">Check in</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">List of items under the column</td>
      <td style="text-align:left">An array of menu items</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Book title</td>
      <td style="text-align:left">The name of the book returned</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">Check-in date</td>
      <td style="text-align:left">The date when the book must be returned</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">Format: dd-mm-yyyy</td>
    </tr>
    <tr>
      <td style="text-align:left">Pay fine</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Penalty for delay or misplacement</td>
      <td style="text-align:left">number</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Add Book</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Include additional books requested</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Report stolen</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Mark missing book</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">New membership</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Include new patron request</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">Format: &#x201C;name, contact_number&#x201D;</td>
    </tr>
    <tr>
      <td style="text-align:left">Cancel membership</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Dismiss patron&#x2019;s membership</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">
        <p>Format:</p>
        <p>&#x201C;name, contact_number&#x201D;</p>
      </td>
    </tr>
  </tbody>
</table>

