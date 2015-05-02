case class TapionTaskulaskin(arvo1 : Double, arvo2 : Double) {
    def plus : Double = this.arvo1 + this.arvo2
    def miinus : Double = this.arvo1 - this.arvo2
    def jako : Double = this.arvo1 / this.arvo2
    def kerto : Double = this.arvo1 * this.arvo2
    def plus (tasku : TapionTaskulaskin) : Double = tasku.arvo1 + tasku.arvo2
}

val t = TapionTaskulaskin(1,2)

println("plussaa: " + t.plus)
println("miinusta: " + t.miinus)
println("kerro: " + t.kerto)
println("jaa: " + t.jako)
println("plussaa olio: " + t.plus(TapionTaskulaskin(1,3)))