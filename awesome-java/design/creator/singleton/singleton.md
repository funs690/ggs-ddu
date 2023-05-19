
``` java
// singleton class
public class Singleton {

    /**
     * private construct
     */
    private Singleton(){

    }

    /**
     * singleton
     */
    private static Singleton singleton;

    /**
     * get object method
     * @return
     */
    public synchronized static Object getInstance(){
        // if not exist, new an instance
        if (singleton == null){
            return new Object();
        }
        return singleton;
    }
    
}

```