# Console progress bar for Scala

Console progress bar for Scala Inspired from [pb](http://github.com/cheggaaa/pb).

## Examples
1. simple example
```scala
object Main {
  def main(args: Array[String]) {
    var count = 1000
    var pb = new ProgressBar(count)
    pb.showSpeed = false
    for (_ <- 1 to count) {
      pb += 1
      Thread.sleep(10)
    }
    println("done")
  }
}
```
