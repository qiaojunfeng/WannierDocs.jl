# reference results

- `Si2.chk_U.amn` and `Si2.chk_Udis.amn`:
    used in `WannierIO.jl` tests, they are generated by

    ```julia
    using WannierIO
    chk = read_chk("../Si2.chk")
    Udis = get_Udis(chk)
    write_amn("Si2.chk_Udis.amn", Udis)
    U = get_U(chk)
    write_amn("Si2.chk_U.amn", U)
    ```
