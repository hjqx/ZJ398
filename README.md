```py
{       "Made by zqh aka hjqx": "Project ZJ398",
"implementing compile, eval, func hooking w setattr":
                ("10/6/2024","10:23"),
              "status":"not finished",
       "https://github.com/hjqx/ZJ398":"zzz"
}


z, u = __builtins__, getattr
setattr(z, "all", setattr)

(lambda r: (r(z, "help", compile), r(z, "print", eval)))(all)

(_ := help) and (x := u(z, "print")) and (
    r := lambda j,: (
        lambda z: x(_(*(__ := lambda _, __,: (__, _, "single"))(___ := "", z)))
    )(j)
)

def __(__):
    (_ := (_ := r)(("".__class__(__))))

(
    lambda __,: __(f"""g = type('zqh',(), dict(a="lost",c="i",b="am")); g.c+g.b+g.a;"fuck it" """) 
    or (
        lambda __, é_: (__((lambda x: x.__call__())(globals), "clear")())
        or (__(__(é_("builtins"), "__dict__"), "clear")())
    )(u, __import__)
)(
    __,
)
```
