[elton.docx](https://github.com/doit01/webclient/files/6987962/elton.docx)
# webclient
https://www.jianshu.com/p/faeb540f30ce

https://www.cnblogs.com/qq931399960/p/13586927.html
retry
mono.subscribe(new MainConsumer(i));


@Override
    public String failureWithFallback() {
    //import io.vavr.control.Try;
        return Try.ofSupplier(this::failure).recover(this::fallback).get();
    }

    private String fallback(Throwable ex) {
        return "Recovered: " + ex.toString();
    }
