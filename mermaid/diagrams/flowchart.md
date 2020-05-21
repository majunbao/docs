```mermaid
graph LR
    Start --> Stop
```

```mermaid
graph LR
    ID
```

```mermaid
graph LR
    id1[This is the text in the box]
```

```mermaid
graph LR
    id1([This is the text in the box])
```


```mermaid
graph LR
    id1[(Database)]
```

```mermaid
graph LR
    id1((Text in the circle))
```

```mermaid
graph LR
    id1>This is the text in the box]
```

```mermaid
graph LR
    id1{This is the text in the box}
```

```mermaid
graph LR
    id1{{This is the text in the box}}
```

```mermaid
graph TD
    id1[/This is the text in the box/]
```

```mermaid
graph TD
    id1[\This is the text in the box\]
```

```mermaid
graph TD
    id1[/This is the text in the box\]
```

```mermaid
graph TD
    id1[\This is the text in the box/]
```

```mermaid
graph LR
    A --> B
```

```mermaid
graph LR
    A --- B
```

```mermaid
graph LR
    A -- This is the text --- B
```

```mermaid
graph LR
    A --- |This is the text| B
```

```mermaid
graph LR
    A --This is the text--> B
```

```mermaid
graph LR
    A -->|This is the text| B
```

```mermaid
graph LR
    A -.- B
```

```mermaid
graph LR
    A -.This is the text.- B
```

```mermaid
graph LR
    A -.This is the text.-> B
```

```mermaid
graph LR
    A ==> B
```

```mermaid
graph LR
    A == text ==> B
```

```mermaid
graph LR
    A -- text --> B -- text2 --> C
```

```mermaid
graph LR
    A --> B & C --> D
```

```mermaid
graph TD
    A & B --> C & D
```

```mermaid
graph TD
    A --> C
    A --> D
    B --> C
    B --> D
```

```mermaid
flowchart TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
    one --> two
    three --> two
    two --> c2
```