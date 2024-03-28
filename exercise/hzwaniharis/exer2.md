## UML diagrams

You can render UML diagrams using [Mermaid](https://mermaidjs.github.io/). For example, this will produce a sequence diagram:

```mermaid
sequenceDiagram
Hayfa ->> Afiq: Hello Afiq, how are you?
Afiq-->>Afiy: How about you Afiy?
Afiq--x Hayfa: I am good thanks!
Afiq-x Afiy: I am good thanks!
Note right of Afiy: Afiq thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

Afiq-->Hayfa: Checking with Afiy...
Hayfa->Afiy: Yes... Afiy, how are you?
```

And this will produce a flow chart:

```mermaid
graph LR
A[Square Rect] -- Link text --> B((Circle))
A --> C(Round Rect)
B --> D{Rhombus}
C --> D
```

```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```
```mermaid
gantt
    title A Gantt Diagram
    dateFormat YYYY-MM-DD
    section Section
        A task          :a1, 2014-01-01, 30d
        Another task    :after a1, 20d
    section Another
        Task in Another :2014-01-12, 12d
        another task    :24d
```
