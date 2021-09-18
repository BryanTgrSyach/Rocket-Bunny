using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class playerMovement : MonoBehaviour
{
    Rigidbody2D Rb;
    public float jumpforce;
    float score;

    void Start()
    {
        Rb = GetComponent<Rigidbody2D>();
    }

    void Update()
    {
        if(Input.GetMouseButtonDown(0))
        {
            Rb.velocity = Vector2.up * jumpforce;
        }
    }

    private void OnTriggerEnter2D(Collider2D collision)
    {
        if(collision.gameObject.tag=="point")
        {
            score++;
        }

        if(collision.gameObject.tag =="pipa")
        {
            Destroy(gameObject);
        }
    }

}
