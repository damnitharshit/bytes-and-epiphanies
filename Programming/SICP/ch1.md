# Chapter 1

### Ex 1.1
```
10
12
8
3
6
No output
No output
19
false
4
16
6
16
```

### Ex 1.2
```scheme
#lang racket

(display (/ (+ 5 4 (- 2 (- 3 (+ 6 (/ 4 5))))) (* 3 (- 6 2) (- 2 7))))
```

### Ex 1.3
```scheme
#lang racket

(define (sum-square-of-larger-nums n1 n2 n3)

  (define (sq x)
    (* x x))

  (define (min a b c)
    (cond
      [(and (< a b) (< a c)) a]
      [(and (< b a) (< b c)) b]
      [(and (< c a) (< c b)) b]))

  (- (+ (sq n1) (sq n2) (sq n3)) (sq (min n1 n2 n3))))

(sum-square-of-larger-nums 1 2 3)
```

### Ex 1.4
```
Adds b to a if b>0, and subtracts b from a otherwise.
```

### Ex 1.5
```
Normal-Order evaluates to 0, while Applicative-Order results in an infinite loop.
```

---