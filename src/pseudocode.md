START
READ a

    IF a == 0 THEN
        PRINT "Not quadratic equation."
    ELSE
        READ b, c
        
        // Calculate the discriminant
        D = (b * b) - (4 * a * c)
        
        IF D == 0 THEN
            PRINT "Two equal roots."
            
        ELSE IF D > 0 THEN
            // Calculate two distinct roots
            x1 = (-b + SQRT(D)) / (2 * a)
            x2 = (-b - SQRT(D)) / (2 * a)
            PRINT "Two different roots: x1=" + x1 + " and x2=" + x2
            
        ELSE
            // Case for D < 0
            PRINT "No real roots"
        END IF
        
    END IF
END