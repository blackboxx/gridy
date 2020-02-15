/*ADAPTIVE DESIGN*/
$mobile: "all and (max-width: 50em)";
$desktop: "all and (min-width: 50em)";
/*END ADAPTIVE DESIGN*/

@mixin base-gridy{
    display: inline-block;
    float: left;
    box-sizing: border-box;
}
.half{
    @include base-gridy();
    width: (100% /2);
    min-width: (100% /2);

}
.half-m{
    @include base-gridy;
    @media #{$mobile} {
        width: 100%;
        float:left;
    }
    @media #{$desktop} {
        width: (100% /2);
        float:left;
    }
}
.one-third{
    @include base-gridy;
    width: (100% /3);
    min-width: (100% /3);

}
.one-third-m{
    @include base-gridy;
    @media #{$mobile} {
        width: 100%;
        float:left;
    }
    @media #{$desktop} {
        width: (100% /3);
        float:left;
    }
}
.one-fourth{
    @include base-gridy;
    width: (100% /4);
    min-width: (100% /4);
}
.one-fourth-m{
    @include base-gridy;
    @media #{$mobile} {
        width: 100%;
        float:left;
    }
    @media #{$desktop} {
        width: (100% /4);
        float:left;
    }
}
.three-fourth{
    @include base-gridy;
    width: (100% /4 *3);
    min-width: (100% /4 *3);
}
.three-fourth-m{
    @include base-gridy;
    @inclide three-fourth;
    @media #{$mobile} {
        width:100%;
    }
    @media #{$desktop} {
        width: (100% /4 *3);
        min-width: (100% /4 *3);
    }
}
