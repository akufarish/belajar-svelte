<script>
    let angka = 0

    $: kali = angka * 5;

    const tambah = () => {
        angka++;
    }

    const reset = () => {
        angka = 0
    }
</script>

<p>{kali}</p>

<button on:click={tambah}>
   Tombol ini telah ditekan sebanyak {angka} kali
</button>


<button on:click={reset}>
    Reset ini agar button kembali jadi nol
</button>