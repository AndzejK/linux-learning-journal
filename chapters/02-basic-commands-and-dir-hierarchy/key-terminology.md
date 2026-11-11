## Streams

1. Standard Input (*stdin*)
e.g. A terminal

2. Standard Output (*stdout*)
e.g. A *text* file/terminal

3. Standard Error (*stderr*)
e.g A *text* file

### **~**: a tilde /*ˈtɪldə*/ - the abbreviation for a **home dir**

### **Expansion**: turning a placeholder / special expression into ist value. 
*Near-synonyms*: 
- Substitution, 
- Replacement,
- **Unfolding**;

```bash
 echo Des*
```

```bash 
* ```: tells the shell to match **any number** of *arbitrary characters*.

```bash 
? 
```: instructs the shell to match **exactly one** *arbitrary character*.

**NOTE**: The shell (*first*) performs expansions **before** running commands, and only then.