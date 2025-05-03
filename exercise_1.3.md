Exercise 1.3: Define a procedure that takes three numbers as arguments and returns the sum of the squares of the two larger numbers.

```lisp
(define (sum-square-two-larger a b c)
      (define (sum-square x y)
        (+ (* x x) (* y y)))
      (cond ((and (< a b) (< a c) (sum-square b c)))
            ((and (< b a) (< b c) (sum-square a c)))
            ((and (< c a) (< c b) (sum-square a b)))))
```