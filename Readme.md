# Ginkgo Sublime Completions

A collection of [Ginkgo](http://github.com/onsi/ginkgo) and [Gomega](http://github.com/onsi/gomega) completions for [Sublime Text](http://sublimetext.com)

## Installation

Use [Package Control](https://sublime.wbond.net/) to search for and install `Ginkgo Completions`.

## Provided Completions

### Ginkgo Completions

#### BDD DSL
```
desc→/Desc→
Describe("", func() {
    
})
```

```
cont→/Cont→
Context("", func() {
    
})
```

```
it→/It→
It("", func() {
    
})
```

```
bef→/Bef→
BeforeEach(func() {
    
})
```

```
jus→/Jus→
JustBeforeEach(func() {
    
})
```

```
aft→/Aft→
AfterEach(func() {
    
})
```

#### Suite lifecycle
```
befs→/Befs→
BeforeSuite(func() {
    
})
```

```
afts→/Afts→
AfterSuite(func() {
    
})
```

```
syncbefs→/Syncbefs→
SynchronizedBeforeSuite(func() []byte {
    //runs on node 1
    return
}, func(node1Data []byte) {
    //runs on all nodes 
})
```

```
syncafts→/Syncafts→
SynchronizedAfterSuite(func() {
    //runs on all nodes
}, func() {
    //runs on node 1 
})
```

#### Measurements
```
meas→/Meas→
Measure("", func(b Benchmarker) {
    
})
```

### Gomega Completions

#### Synchronous assertions
```
Ω→
Ω().Should(Equal())
```

```
Ωerr→
Ω(err).ShouldNot(HaveOccurred())
```

```
ex→/Ex→
Expect().To(Equal())
```

```
exerr→/Exerr→
Expect(err).NotTo(HaveOccurred())
```


#### Asynchronous Assertions
```
ev→/Ev→
Eventually().Should(Equal())
```

```
evf→/Evf→
Eventually(func() interface{} {
    return
}).Should(Equal())
```

```
cons→/Cons→
Consistently().Should(Equal())
```

```
consf→/Consf→
Consistently(func() interface{} {
    return
}).Should(Equal())
```
